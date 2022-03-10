# contentstation-drag-to-indesign
This integration adds a custom button to the Dossier panel which can be dragged to InDesign. When dropped the selected files are placed or loaded in the InDesign place gun.

![Drag & drop in action](https://github.com/WoodWing/contentstation-drag-to-indesign/blob/master/drag-to-indesign.gif "Drag & drop in action")

# Configuration
For production purposes deploy the dragToInDesign.js to a public location and configure it in the [Studio Management console](https://helpcenter.woodwing.com/hc/en-us/articles/4404782940561-Managing-plug-ins-in-Studio)

For **DEMO** purposes the plugin could also be loaded from https://woodwing.github.io/contentstation-drag-to-indesign/dragToInDesign.js. Availability is however not guaranteed.


# Notes
* The plugin assumes that the server URL returned by the Content Station SDK matches the server URL configured for InDesign. Please update the createDragData function if this is not the case. 
* The text of the button and tooltip can be localized by changing the D2ID_LABEL and D2ID_HINT_TEXT constants
