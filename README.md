# nightmare-pdf-cli
Easy PDF Generation CLI using nigthmarejs


## Dependencies

This CLI depends on [Nightmare](https://github.com/segmentio/nightmare), you need to first install it using `npm`:

`npm install nightmare`

*Warning*, as of today, getting nightmare (which depends on Electron) to work on linux is not that easy.

# Usage

`node rasterize.js url filename [--timeout] [--pageSize] [--landscape] [--printBackground] [--marginsType]`

+ url [required]
+ filename [required] the name of the generated PDF (eg. 'my_document.pdf')
+ timeout [Optional] default to 1000, defines the timeout between the opening and the rendering of the url by nightmare
+ pageSize [Optional] default to 'A4', accepts options are A3, A4, A5, Legal, Letter or Tabloid
+ landscape [Optional] default to 0, defines whether rendering pdf in landscape mode
+ printBackground [Optional] default to 1, defines whether printing background
+ marginsType [Optional] default to 1, defines which margins to use. Uses 0 for default margin, 1 for no margin, and 2 for minimum margin.