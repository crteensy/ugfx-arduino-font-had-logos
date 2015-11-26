# ugfx-arduino-font-had-logos
Hackaday logos font for ugfx-arduino

## Included glyphs
As of now there's just the hackaday prize glyph (wrenched skull with astronaut helmet) with 98 pixels height in had-logos-98 at character code 'H' (hex 0x48, decimal 72)

## Installation
Put the whole library into your sketchbook library directory

## Usage
- enable user fonts in your gfxconf.h:

    ```C++
#define GDISP_NEED_TEXT             TRUE    
#define GDISP_INCLUDE_USER_FONTS    TRUE
    ```

- create userfonts.h in your project-specific config library (if not present already), add

```C++
#include "ugfx-arduino-font-had-logos.h"
```

- in your sketch, load the font with

```C++
font_t logofont = gdispOpenFont("had-logos-98"); // height 98 pixels, see fontdata/*.c for font names
```
