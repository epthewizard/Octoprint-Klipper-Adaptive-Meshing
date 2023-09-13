# Octoprint-Klipper-Adaptive-Meshing
This repo includes the instructions to get KAMP working on your printer running Klipper and Octoprint

### Instructions
1. Head over to the [KAMP](https://github.com/kyleisah/Klipper-Adaptive-Meshing-Purging) repo and follow the guide to setup KAMP with Klipper.
2. Once setup, follow the steps from [this](https://github.com/kageurufu/preprocess_cancellation) repo to setup preprocessing for your slicer.

   **Note:** If you are using Cura, you need to open the scripts folder within the main Cura installation folder. This can be accessed by going to _Help -> Show Configuration Folder._ Make sure to add the preprocess_cancellation.py file to your scripts folder and the binary for your machine in the main Cura folder.
4. Once both are setup, you can then put your model in the slicer and add the postprocessing script that will send the objects coordinates to Klipper. Then slice away and KAMP should be working.

### Troubleshooting
- If your printer is doing a mesh of your entire bed make sure to add *M117* to the first line of your start GCODE.
