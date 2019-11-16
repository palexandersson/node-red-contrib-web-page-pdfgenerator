# node-red-contrib-web-page-screenshot
A Node-RED node for generating pdf's of web pages.

## Install 

```
cd ~/.node-red
npm install node-red-contrib-web-page-pdfgenerator
```

## Usage

 - Supply url of web page to be converted to pdf.

## Settings


### Name (Optional)

You can set any name to the node. Blank is allowed.

### Web Page URL (Optional)

URL which you want to take a screenshot. If blank, this node will take a screenshot of http://example.com .

### executablePath (Optional)

You can specify chromium/chrome executable with the path. For those who use x86 arch, this can be blank, however, if you use this node on ARM arch (e.g. Raspberry Pi), you have to install headless-mode-available `chromium-browser` and set the path.

> Fortunately, [Raspbian OS](https://www.raspberrypi.org/downloads/raspbian/) (as of ver. April 2019) includes compatible `chromium-browser`, so just set `/usr/bin/chromium-browser` to this blank.

## Example


This flow provides a web page with a screenshot of a configured URL.


## Details and Issues

 - This node uses `puppeteer` for generating pdf's.
