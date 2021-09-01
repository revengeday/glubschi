# 👀 Glubschi 
Easily convert text in images to raw text (OCR).

# Install via Chrome Webstore
In review by Google (since 2021-09-01)

# Installation guide for Chromium based browsers
You can easily create your own version of this extension.
All you need is time and some understanding of browser extension development.

- Read the developer documentation from your browser manufacturer
- Create a manifest (V3) document (mostly a .json document)

Here is an example for Chromium based browsers:

```{
   "action": {

   },
   "background": {
      "service_worker": "worker.js"
   },
   "description": "",
   "homepage_url": "https://github.com/revengeday",
   "icons": {
      "128": "data/icons/128.png",
      "16": "data/icons/16.png",
      "256": "data/icons/256.png",
      "32": "data/icons/32.png",
      "48": "data/icons/48.png",
      "512": "data/icons/512.png",
      "64": "data/icons/64.png"
   },
   "manifest_version": 3,
   "minimum_chrome_version": "90",
   "name": "Glubschi",
   "permissions": [ "storage", "activeTab", "scripting" ],
   "update_url": "https://clients2.google.com/service/update2/crx",
   "version": "0.0.4.3",
   "web_accessible_resources": [ {
      "matches": [ "*://*/*" ],
      "resources": [ "data/ui/index.html" ]
   } ]
}
```

# Third party libarys
[Tesseract OCR](https://www.npmjs.com/package/node-tesseract-ocr) is used locally in this Chrome extension within the chrome storage.


