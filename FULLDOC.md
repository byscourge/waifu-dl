FULLDOC.md: Full documentation of waifu-dl.


## CLI Docs:
*  waifu --help: Show this help screen
*  waifu --nsfw help: Show nsfw help screen
*  waifu --view help: Show image viewer help screen
*  waifu --output --help: Show output-save help screen
*  waifu --id help: Show id lookup help screen
*  waifu --tag help: Show tag lookup help screen
*  waifu --exclude help: Show tag exclusion help screen
*  waifu --type help: Show type sort help screen
*  waifu --sort help: Show sort type help screen
*  waifu --orientation help: Show orientation sort help screen
*  waifu --chafa-format help: Show chafa type help screen
*  waifu --unihelp: Show all help screens

## Valid flags (18):
*  waifu -h/--help [ Show help screen ]
*  waifu --unihelp [ Print all help screens at once ]
*  waifu -t/--termux [ Android: open media with termux-open ]
*  waifu -p/--print [ Print URL ]
*  waifu --no-print [ Force-disable stdout printing ]
*  waifu --raw [ Print pre-curl waifu.im URL ]
*  waifu --json [ Print pre-jq waifu.im JSON ]

*  waifu -o/--output (arg required) [ Save output as filename.ext ]
*  waifu -n/--nsfw (arg required) [ Set NSFW Mode ]
*  waifu -v/--view (arg required) [ Set inline image viewer mode ]
*  waifu -i/--id (arg required) [ Lookat specific waifu ID ]
*  waifu -g/--tag (arg required) [ Set included tag ]
*  waifu -G/--exclude (arg required) [ Set excluded tag ]
*  waifu -a/--type (arg required) [ Set media type ]
*  waifu -s/--sort (arg required) [ Set sort type ]
*  waifu -r/--orientation (arg required) [ Set orientation type ]
*  waifu --chafa-format (arg required) [ Set override chafa encode type ]
*  waifu --print-var (arg required) [ Print internal waifu variable ]

## Require-argument flags:

waifu: --nsfw

Set NSFW mode

Valid options:

  * e (exclusive) [ Set to only NSFW media ]
  * b (both) [ Set to both NSFW and SFW media ]
  * a (all)  [ Set to both NSFW and SFW media ]
  * n (none) [ Set to no NSFW media ]
  
--------------------------------

waifu: --view

Set VIEW mode

Valid options:

  * c (chafa) [ Set to view with Chafa ]
  * s (sixel) [ Set to view with Img2sixel ]

--------------------------------

waifu: --output

Save media as FILENAME.ext

Usage:

  waifu -o file [ Appends extension automatically ]


--------------------------------

waifu: --id

View an image from a specific ID ( any number up to 4 digits )

Usage:
  waifu -i xxxx (numbers)

ID examples:
  1739 3119 5469 5943 6162 6873 6900 6992 7124 7727 7799 8357

you can also use any other number. these are working examples, though (real waifu id's), so feel free to use these aswell.

--------------------------------

waifu: --tag

Set TAG filter

Valid tags:

  milf, uniform, ass, maid,
  waifu, ero, ecchi, oppai, hentai,
  selfies, paizuri, oral, rem,

  raiden-shogun, marin-kitagawa,
  mori-calliope, kamisato-ayaka,
  genshin-impact, nami, one-piece

--------------------------------

waifu: --exclude

Set TAG to exclude

Valid tags:

  milf, uniform, ass, maid,
  waifu, ero, ecchi, oppai, hentai,
  selfies, paizuri, oral, rem,

  raiden-shogun, marin-kitagawa,
  mori-calliope, kamisato-ayaka,
  genshin-impact, nami, one-piece

--------------------------------

waifu: --type

Set TYPE filter (animated vs static images)

Valid options:

  * a (animated) [ Only animated (gif) media ]
  * s (static)   [ Only static (non-gif) media ]
  * b (both), all [ Both animated and static media ]

--------------------------------

waifu: --sort

Set SORT order

Valid options:

  * f (favorites), p (popular) [ Sort by most popular ]
  * u (uploaded), n (newest)   [ Sort by newest upload ]
  * r (random)                 [ Sort randomly (default if --sort is omitted) ]

--------------------------------

waifu: --orientation

Set ORIENTATION filter

Valid options:

  * l (landscape) [ Landscape images only ]
  * p (portrait)  [ Portrait images only ]
  * s (square)    [ Square images only ]
  * a (all)       [ Any orientation ]
    
--------------------------------

waifu: --chafa-format

Use chafa specifically & specify the format

Usage:

  waifu --chafa-format [format]

Valid formats:

  iterm kitty sixels symbols

--------------------------------


## Exit codes for scripting:
* Exit-code 1: Generic error

* Exit-code 2: Missing core command
* Exit-code 3: Missing other/optional command
* Exit-code 4: Getopt is not GNU
* Exit-code 5: Failed argument/paremeter parsing
* Exit-code 6: Failed to fetch valid media data
* Exit-code 7: Invalid variable name (part of --print-var)

## waifu-dl Has a killswitch mechanism:
* It uses the same approach as hushlogin, if ~/.waifulock exists, it exits with no action.
