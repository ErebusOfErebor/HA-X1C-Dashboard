# HomeAssistant BambuLab Printer Dashboard

My own custom dashboard for my BambuLab printer.

## What Printers does this work for?

I made this dashboard specifically for my use case, which is an X1C with one AMS unit. Though adaptations can likely be made for various users and use cases.

## What is needed for this dashboard?

HACS
* Bubble Card
* Mushroom
* hui-element
* button-card
* layout-card
* custom-brand-icons
* webrtc-camera
* card-mod


[Bambu NodeRed Integration](https://github.com/WolfwithSword/Bambu-HomeAssistant-Flows/tree/main) by [WolfWithSword](https://www.wolfwithsword.com). This may work with the HACS Integration, but I do not use that and have not tested this dashboard with it.

A few custom images that Wolf has supplied. The humidity-level icons can be found [here](https://github.com/WolfwithSword/Bambu-HomeAssistant-Flows/tree/main/files/media/custom_icons), and the image for your specific printer found [here](https://github.com/WolfwithSword/Bambu-HomeAssistant-Flows/tree/main/files/media/www/media/bambuprinter). Thanks to Wolf again for making these easy for me to get.

An Input Boolean named "3D Printer End Time Switch". Mine has the entity id `input_boolean.3d_printer_end_time_switch`. This is used to switch the display value of the End Time between absolute (e.g. 18:30) and relative (e.g. 1h36m)

## Additional Notes/Info
I have an Aqara Temp & Humidity sensor inside my AMS unit in the back, which is how I'm getting the actual Temperature and Humidity % in the dashboard. I'm using [this](https://makerworld.com/en/models/687462?from=search#profileId-616147) holder by [Piitaya](https://makerworld.com/en/@Piitaya).

I have the solid black image as a background on the picture-elements card. This allows me to display the temperatures on top of the camera. I could use the default Generic Camera integration with the picture-elements card, but I find this to be slower to low and delayed.