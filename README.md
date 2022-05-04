# Metrology for Home Assistant
A collection of themes, tweaks, and template buttons to make your Home Assistant look modern and clean. Based on Metro UI Design System.

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/madelena)

## Metro Theme

![Collage of Screenshots showing the Metro theme in light and dark modes](/examples/HA%20Metrology%20-%20Metro%20Theme%20-%20Collage.png)

### Features

- Uses Segoe UI or Segoe UI Variable fonts with a distinct and bold typography.
- Supports Light and Dark Modes natively. Dark Mode has a true black background great for AMOLED screens.
- Includes 4 Themes. Also adding new themes is relatively easy thanks to YAML Anchors.
- Revamps the More Info card and various system UI screens.

### Screenshots

|   |   |   |   |
|--- | --- | ---| ---|
| ![Red Theme (Light)](/examples/HA%20Metrology%20-%20Color%20Themes%20-%20Red%20(Light).png) | ![Orange Theme (Light)](/examples/HA%20Metrology%20-%20Color%20Themes%20-%20Orange%20(Light).png) | ![Green Theme (Light)](/examples/HA%20Metrology%20-%20Color%20Themes%20-%20Green%20(Light).png) | ![Blue Theme (Light)](/examples/HA%20Metrology%20-%20Color%20Themes%20-%20Blue%20(Light).png) |
| ![Red Theme (Dark)](/examples/HA%20Metrology%20-%20Color%20Themes%20-%20Red%20(Dark).png) | ![Orange Theme (Dark)](/examples/HA%20Metrology%20-%20Color%20Themes%20-%20Orange%20(Dark).png) | ![Green Theme (Dark)](/examples/HA%20Metrology%20-%20Color%20Themes%20-%20Green%20(Dark).png) | ![Blue Theme (Dark)](/examples/HA%20Metrology%20-%20Color%20Themes%20-%20Blue%20(Dark).png) |
| ![Device Example (Dark)](/examples/HA%20Metrology%20-%20Device%20Example%20(Dark).png) Device Example | ![Device Example (Light)](/examples/HA%20Metrology%20-%20Device%20Example%20(Light).png) Device Example | ![Binary Sensor Example (Dark)](/examples/HA%20Metrology%20-%20More%20Info%20Box%20Example%20-%20Binary%20Sensor%20(Dark).png) Binary Sensor Example | ![Device Example (Dark)](/examples/HA%20Metrology%20-%20More%20Info%20Box%20Example%20-%20Binary%20Sensor%20(Light).png) Binary Sensor Example | 
| ![Update (Dark)](/examples/HA%20Metrology%20-%20More%20Info%20Box%20Example%20-%20Update%20(Dark).png) Update Example | ![Update (Light)](/examples/HA%20Metrology%20-%20More%20Info%20Box%20Example%20-%20Update%20(Light).png) Update Example | ![Sensor Example (Dark)](/examples/HA%20Metrology%20-%20More%20Info%20Box%20Example%20-%20Sensor%20(Dark).png) Sensor Example | ![Sensor Example (Dark)](/examples/HA%20Metrology%20-%20More%20Info%20Box%20Example%20-%20Sensor%20(Light).png) Sensor Example | 
| ![Settings Example](/examples/HA%20Metrology%20-%20Settings%20Example%20(Light).png) Settings Example | | | |
| | | |

### How to Install the Theme

If you have HACS, you probably already know what you are doing. You can search for this theme and install it there. If you don't have HACS, here are the steps:

Prerequisites:

- Some way to upload files to your HA server, e.g. Visual Studio Code or Samba add-ons
- card-mod

Installation:

- Add this in your configuration.yaml file:

```
frontend:
  themes: !include_dir_merge_named themes
```

- Create a new folder named `themes` under `/config`.
- Copy `metro.yaml` to `/config/themes`.
- (Optional if you want Segoe UI on non-Windows devices) Copy `style.css` and the `.ttf` font files to `/www`.
- Restart Home Assistant to apply the changes.
- Go to your Profile page, which is the button where your avatar is at the bottom left.
- Under Themes, choose the color you like for the Metro themes.
- Pick Auto, Light, or Dark Mode for the theme.

Segoe UI font is optional if you are already using Windows. If you are not using Home Assistant, you can download the fonts [here](https://docs.microsoft.com/en-us/windows/apps/design/downloads/#fonts) and upload them along with style.css to your /config/www folder.

## Card Templates

TBD. Includes button-card templates in the form of Live Tiles.

### Title Card


### Header Card


### Live Tile


### Live Tile Card


### Live Tile Media Player Card


### Mini Graph Card


### Light Group Card


### Light Slider Card


### Hue Scene Card and Card Mini


### How to use wider Live Tiles


### CSS Variables for your custom cards



## See Also

Metrology is a suite of themes inspired by Metro UI Design System to make your system look distinctively bold and clean.

- [Metrology for Musicbee](https://github.com/Madelena/Metrology-for-Musicbee)
