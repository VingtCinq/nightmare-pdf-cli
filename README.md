# nightmare-pdf-cli
Easy PDF Generation CLI using nigthmarejs


## Dependencies

This CLI depends on [Nightmare](https://github.com/segmentio/nightmare), you need to first install it using `npm`:

`npm install nightmare`

*Warning*, as of today, getting nightmare (which depends on Electron) to work on linux is not that easy.

# Usage

`node rasterize.js url filename [--timeout] [--page_size] [--landscape] [--print_background] [--margins_type]`

+ url [required]
+ timeout [Optional] default to 1000, defines the timeout between the opening and the rendering of the url by nightmare
+ page_size [Optional] default to 'A4', accepts options are A3, A4, A5, Legal, Letter or Tabloid
+ landscape [Optional] default to 0, defines whether rendering pdf in landscape mode
+ print_background [Optional] default to 1, defines whether printing background
+ margins_type [Optional] default to 1, defines which margins to use. Uses 0 for default margin, 1 for no margin, and 2 for minimum margin.