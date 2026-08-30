
## ***waifu-dl is a CLI tool: view or download random waifu images from 'waifu.im'.***

#### Use the script's CLI --help option/suboptions for more info.

## Docs:
*  waifu --help: Show this help screen
*  waifu --nsfw help: Show nsfw help screen
*  waifu --view help: Show image viewer help screen
*  waifu --id help: Show id lookup help screen
*  waifu --tag help: Show tag lookup help screen
*  waifu --type help: Show type sort help screen
*  waifu --sort help: Show sort type help screen
*  waifu --orientation help: Show orientation sort help screen

## Usage examples:
*  waifu -ne -o animegirl.png [ Set mode to only NSFW and save the image to ./animegirl.png ]
*  waifu -nb -t [ Set mode to all (NSFW+SFW) and open it with termux-open, for termux users. ]
*  waifu -ne -vc [ Set mode to only NSFW and view the image with chafa ]
*  waifu -p [ Print image URL ]
*  waifu -vc -ne -ghentai [ Set mode to only NSFW, search the tag hentai and view the image with chafa ]
*  waifu -vc -nn -gwaifu [ Set mode to no NSFW, search the tag waifu and view the image with chafa ]

## Valid flags (13):

*  waifu -h/--help [ Show help screen ]
*  waifu -t/--termux [ Android: open media with termux-open ]
*  waifu -p/--print [ Print URL ]
*  waifu --no-print [ Force-disable URL printing ]
*  waifu --unihelp [ Print all help screens at once ]

*  waifu -o/--output (arg required) [ Save output as filename ]
*  waifu -n/--nsfw (arg required) [ Set NSFW Mode ]
*  waifu -v/--view (arg required) [ Set inline image viewer mode ]
*  waifu -i/--id (arg required) [ Lookat specific waifu ID ]
*  waifu -g/--tag (arg required) [ Set included tag ]
*  waifu -a/--type (arg required) [ Set media type ]
*  waifu -s/--sort (arg required) [ Set sort type ]
*  waifu -r/--orientation (arg required) [ Set orientation type ]

## All options in action:
*  waifu --nsfw=exclusive --view=chafa --tag=hentai --type=static --sort=popular --orientation=portrait --no-print

Short:
*  waifu -ne -vc -ghentai -as -sp -rp --no-print


## Installation
```bash
wget https://raw.githubusercontent.com/byscourge/waifu-dl/master/waifu && chmod +x waifu
```

## Dependencies
* The core is curl & jq, optionally chafa/sixel.
