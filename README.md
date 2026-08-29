
waifu is a simple CLI tool: view or download random waifu images from waifu.im.

Docs:
  waifu --help: Show this help screen
  waifu --nsfw help: Show nsfw help screen
  waifu --view help: Show image viewer help screen
  waifu --id help: Show id lookup help screen

Usage examples:
  waifu -ne -o animegirl.png [ Set mode to only NSFW and save the image to ./animegirl.png ]
  waifu -nb -t [ Set mode to all (NSFW+SFW) and open it with termux-open, for termux users. ]
  waifu -ne -vc [ Set mode to only NSFW and view the image with chafa ]
  waifu -p [ Print image URL ]


Valid flags:

Short:
  waifu -h
  waifu -o (arg required)
  waifu -n (arg required)
  waifu -t
  waifu -v (arg required)
  waifu -p
  waifu -i (arg required)
Long:
  waifu --help
  waifu --output (arg required)
  waifu --nsfw (arg required)
  waifu --termux
  waifu --view (arg required)
  waifu --print
  waifu --id (arg required)
  

