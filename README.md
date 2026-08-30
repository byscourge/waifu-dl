
waifu is a simple CLI tool: view or download random waifu images from waifu.im.

#### Use the script's CLI --help option/suboptions for more info.

Docs:
  waifu --help: Show the help screen
  waifu --nsfw help: Show nsfw help screen
  waifu --view help: Show image viewer help screen
  waifu --id help: Show id lookup help screen
  waifu --tag help: Show tag lookup help screen

Usage examples:
  waifu -ne -o animegirl.png [ Set mode to only NSFW and save the image to ./animegirl.png ]
  waifu -nb -t [ Set mode to all (NSFW+SFW) and open it with termux-open, for termux users. ]
  waifu -ne -vc [ Set mode to only NSFW and view the image with chafa ]
  waifu -p [ Print image URL ]
  waifu -vc -ne -ghentai [ Set mode to only NSFW, search the tag hentai and view the image with chafa ]
  waifu -vc -nn -gwaifu [ Set mode to no NSFW (only SFW), search the tag waifu and view the image with chafa ]
 -g is equivalent to --tag

## Installation
```bash
wget https://raw.githubusercontent.com/byscourge/waifu-dl/master/waifu-dl -O waifu && chmod +x waifu
```

## Dependencies
* Almost none! the core is just curl and jq. and (OPTIONALLY) chafa/sixel
