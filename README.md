* This project is licensed under the GNU General Public License v3.0 LICENSE.

## ***waifu-dl is a CLI tool: view or download random waifu images from 'waifu.im'.***

#### Use the script's CLI --help option/suboptions for more info.

## Docs:
*  waifu --help: Show this help screen
*  waifu --nsfw help: Show nsfw help screen
*  waifu --view help: Show image viewer help screen
*  waifu --output help: Show saveas help screen
*  waifu --id help: Show id lookup help screen
*  waifu --tag help: Show tag lookup help screen
*  waifu --exclude help: Show tag exclusion help screen
*  waifu --type help: Show type sort help screen
*  waifu --sort help: Show sort type help screen
*  waifu --orientation help: Show orientation sort help screen

* waifu --unihelp: Show all help screens

## Usage examples:
*  waifu -ne -o animegirl.png [ Set mode to only NSFW and save the image to ./animegirl.png ]
*  waifu -nb -t [ Set mode to all (NSFW+SFW) and open it with termux-open, for termux users. ]
*  waifu -ne -vc [ Set mode to only NSFW and view the image with chafa ]
*  waifu -p [ Print image URL ]
*  waifu -vc -ne -ghentai [ Set mode to only NSFW, search the tag hentai and view the image with chafa ]
*  waifu -vc -nn -gwaifu [ Set mode to no NSFW, search the tag waifu and view the image with chafa ]

## Valid flags (15):

*  waifu -h/--help [ Show help screen ]
*  waifu --unihelp [ Print all help screens at once ]
*  waifu -t/--termux [ Android: open media with termux-open ]
*  waifu -p/--print [ Print URL ]
*  waifu --no-print [ Force-disable URL printing ]

*  waifu -o/--output (arg required) [ Save output as filename ]
*  waifu -n/--nsfw (arg required) [ Set NSFW Mode ]
*  waifu -v/--view (arg required) [ Set inline image viewer mode ]
*  waifu -i/--id (arg required) [ Lookat specific waifu ID ]
*  waifu -g/--tag (arg required) [ Set included tag ]
*  waifu -G/--exclude (arg required) [ Set excluded tag ]
*  waifu -a/--type (arg required) [ Set media type ]
*  waifu -s/--sort (arg required) [ Set sort type ]
*  waifu -r/--orientation (arg required) [ Set orientation type ]
*  waifu --print-var (arg required) [ Print internal waifu variable ]

## All options in action:
*  waifu --nsfw=exclusive --view=chafa --tag=hentai --exclude=ecchi --type=static --sort=popular --orientation=portrait --no-print

Short:
*  waifu -ne -vc -ghentai -as -sp -rp --no-print

## waifu-dl Has a killswitch mechanism:
* It uses the same approach as hushlogin, if ~/.waifulock exists, it prints a friendly message and exits.
* Said message: "This command does nothing. Have a wonderful day!"

## Automation examples:
* Download 20 images
```bash
for i in {1..20}; do
    waifu -ne -sr -as -o "waifu_$i" # Automatically appends extension
done
```

## Installation
```bash
wget https://raw.githubusercontent.com/byscourge/waifu-dl/master/waifu && chmod +x waifu
```

## Dependencies
* The core is curl & jq, optionally chafa/sixel.
* GNU Getopt (>v4.0) is required.
