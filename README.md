# contentstation-drag-to-indesign
This integration adds a custom button to the Dossier panel which can be dragged to InDesign. When dropped the selected files are placed or loaded in the InDesign place gun.

![Drag & drop in action](https://github.com/WoodWing/contentstation-drag-to-indesign/blob/master/drag-to-indesign.gif "Drag & drop in action")

# Installation
1. Place the `dragToInDesign.js` into a subdirectory where you host the Content Station extensions. I.E. `../Enterprise/contentstation-integrations/dragToInDesign.js`
2. Add the URL to the `dragToInDesign.js` into the to the 'contentStation' section of the Content Station [config.js](https://helpcenter.woodwing.com/hc/en-us/articles/115005560243-Configuring-Content-Station-Aurora)
```javascript
    ...
    ...
    plugins: {
        contentStation: [
            // 'sdk/samples/sample-1.js',
            // 'sdk/samples/sample-2.js'
            '../Enterprise/contentstation-integrations/dragToInDesign.js'
        ],
        digitalEditor: [
            // 'sdk/samples/digital-editor-sdk-sample.js',
    ...
    ...
```

# Notes
* The plugin assumes that the server URL returned by the Content Station SDK matches the server URL configured for InDesign. Please update the createDragData function if this is not the case. 
* The text of the button and tooltip can be localized by changing the D2ID_LABEL and D2ID_HINT_TEXT constants
