# What's new/changed?


1. Supports multiple AMS units
2. Redesigned filament popups
3. Icon in Settings/Info popover is dynamic, needs all printer images from Wolf [here](https://github.com/WolfwithSword/Bambu-HomeAssistant-Flows/tree/main/files/media/www/media/bambuprinter).
4. Dropped usage of `webrtc-camera` and `bar-card`


I've also made some parts user-customizeable.
Within the AMS cards there are two variables: `low_filament_threshold` and `has_secondary_temp_and_hum_sensor`.


#### low_filament_threshold
The percentage remaining of your spool at which a red pulsing animation will trigger, indicating the filament is low.

#### has_secondary_temp_and_hum_sensor
I have an Aqara Temp & Humidity sensor in my AMS unit.
If you have something similar, you can set this to true and change the entities to whatever your external sensors are and use those values next to the humidity icon.
If you do not have any external temp and humidity sensors, change this to `false` and it will use the temperature sensor provided from the NodeRed flow and will only use the icon for the humidity, without a separate reading.

<table>
    <tbody>
        <tr>
            <td>
                <img src="https://github.com/ErebusOfErebor/HA-X1C-Dashboard/blob/main/dashboard_images/v2_dashboard.jpeg?raw=true">
            </td>
            <td>
                <img src="https://github.com/ErebusOfErebor/HA-X1C-Dashboard/blob/main/dashboard_images/v2_ams_popup.jpeg?raw=true">
            </td>
        </tr>
    </tbody>
</table>