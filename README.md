DigistumpArduino (Multi-Keyboard Layout MOD)
============================================

Files to add Digistump support (Digispark, Pro, DigiX) to Arduino 1.6.X (1.6.4+)

**These files are designed for install via the Arduino Boards Manager:** 

Board manager URL: http://digistump.com/package_digistump_index.json

### Full Install Instructions:

Digispark: http://digistump.com/wiki/digispark/tutorials/connecting

Digispark Pro: http://digistump.com/wiki/digispark/tutorials/connectingpro

DigiX: http://digistump.com/wiki/digix/tutorials/software

### To compile:

Micronucleus is the only executable in these packages that is pre-compiled:

Micronucleus: https://github.com/micronucleus/micronucleus/tree/80419704f68bf0783c5de63a6a4b9d89b45235c7
Dependencies: libusb and possibly lib32stdc on linux - (on ubuntu get it by issuing: apt-get install lib32stdc++6)

### Using Keyboard Layouts

To specify a custom keyboard layout you have to define a macro previous to include DigiKeyboard.h. 
For example this code will be using Spanish Layout

```c
#define LAYOUT_SPANISH
#include "DigiKeyboard.h"
```

Here is a complete list of all available Layouts:

```c
//#define LAYOUT_US_ENGLISH                 // DEFAULT
//#define LAYOUT_CANADIAN_FRENCH
//#define LAYOUT_CANADIAN_MULTILINGUAL
//#define LAYOUT_DANISH
//#define LAYOUT_FINNISH
//#define LAYOUT_FRENCH
//#define LAYOUT_FRENCH_BELGIAN
//#define LAYOUT_FRENCH_SWISS
//#define LAYOUT_GERMAN
//#define LAYOUT_GERMAN_MAC
//#define LAYOUT_GERMAN_SWISS
//#define LAYOUT_ICELANDIC
//#define LAYOUT_IRISH
//#define LAYOUT_ITALIAN
//#define LAYOUT_NORWEGIAN
//#define LAYOUT_PORTUGUESE
//#define LAYOUT_PORTUGUESE_BRAZILIAN
//#define LAYOUT_SPANISH
//#define LAYOUT_SPANISH_LATIN_AMERICA
//#define LAYOUT_SWEDISH
//#define LAYOUT_TURKISH
//#define LAYOUT_UNITED_KINGDOM	
//#define LAYOUT_US_INTERNATIONAL
```

### Acknowledgments

- [@PaulStoffregen](https://github.com/PaulStoffregen) (PJRC) - For Teensy's implementation of layouts
