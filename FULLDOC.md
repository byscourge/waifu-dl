FULLDOC.md: Documentation of all other flags that require an argument, and how to use them.

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

View an image from a specific ID ( 4-digit number )

Usage:
  waifu -i xxxx (numbers)

ID examples:
  1739 3119 5469 5943 6162 6873 6900 6992 7124 7727 7799 8357

# you can also use any other number. these are working examples, though (REAL IMAGES), so feel free to use these aswell.

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
