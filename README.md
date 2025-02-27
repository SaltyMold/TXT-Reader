# TXT-Reader
This app is a [TXT](https://en.wikipedia.org/wiki/Text_file) reader that runs on the [NumWorks calculator](https://www.numworks.com).

## Install the app

To install this app, you'll need to:
1. Download the latest `TXT-Reader.nwa` file from the [Releases](https://github.com/SaltyMold/TxtReader/releases) page
2. Choose a `txt` file you want to read on your calculator.
3. Connect your NumWorks calculator to your computer using a USB cable.  
4. Head to [my.numworks.com/apps](https://my.numworks.com/apps) to send the `nwa` file on your calculator along the `txt` file.

## How to use the app
| Touche     | Action    |
|------------|----------|
| Back | Quit  |
| Arrow Down | Down |
| Arrow Up | Up |

## Build the app

To build this sample app, you will need to install the [embedded ARM toolchain](https://developer.arm.com/Tools%20and%20Software/GNU%20Toolchain) and [Node.js](https://nodejs.org/en/) 18. The C SDK for Epsilon apps is shipped as an npm module called [nwlink](https://www.npmjs.com/package/nwlink) v0.0.16.

```sh
#debian

sudo apt install -y build-essential git imagemagick libx11-dev libxext-dev \
    libfreetype6-dev libpng-dev libjpeg-dev pkg-config gcc-arm-none-eabi \
    binutils-arm-none-eabi nodejs npm  
npm install -g n  
sudo n 18  
npm install -g nwlink@0.0.16
```

You should now have a `output/app.nwa` file that you can distribute! Anyone can now install it on their calculator from the [NumWorks online uploader](https://my.numworks.com/apps).

## Special thanks 

I followed the guide from [epsilon-sample-app-c](https://github.com/numworks/epsilon-sample-app-c) to build this app.
