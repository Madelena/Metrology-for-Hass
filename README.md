![Collage of Screenshots showing the Metro theme in light and dark modes](https://raw.githubusercontent.com/Madelena/Metrology-for-Hass/main/examples/HA%20Metrology%20-%20Metro%20Theme%20-%20Collage.png)

# Metrology for Home Assistant

Metrology is a practical series of app customizations and redesigns aimed at bringing a bold, clear, and consistent user experience to [various Windows and Android apps](https://github.com/Madelena?tab=repositories&q=Metrology). Its design language is based on [Metro](https://en.wikipedia.org/wiki/Metro_(design_language)) and [Fluent](https://www.microsoft.com/design/fluent/) design systems pioneered by Microsoft Design since the 2010s.

[Home Assistant](https://www.home-assistant.io/) is an open source home automation server that integrates nearly 2000 existing IoT services into one powerful, private, and unified user interface. It is perfect to run on a Raspberry Pi or a local server.

Here is a collection of themes, tweaks, and template buttons to make your Home Assistant look bold, modern, and clean.

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/madelena)

## Table of Contents

- [Metro Theme](#metro-theme)
  - [Screenshots](#screenshots)
  - [How to Install the Theme](#how-to-install-the-theme)
- [Live Tile Templates](#live-tile-templates)
- [Credits](#credits)

## Metro Theme

### Awesome Features

<table>
  <tr width="50%">
    <td>Display your home automation status with distinct and bold typography using Segoe UI or Segoe UI Variable fonts. <img alt="Typography" src="https://raw.githubusercontent.com/Madelena/Metrology-for-Hass/main/examples/Metro%20Theme%20Thumbnail%201.png"/></td>
    <td>Use Light and Dark Modes natively. Dark Mode has a true black background great for AMOLED screens. <img alt="Light and Dark Modes" src="https://raw.githubusercontent.com/Madelena/Metrology-for-Hass/main/examples/Metro%20Theme%20Thumbnail%202.png"/></td>
  </tr>
  <tr width="50%">
    <td>Switch between 4 color themes. Also adding new themes is relatively easy thanks to YAML Anchors. <img alt="Color Themes" src="https://raw.githubusercontent.com/Madelena/Metrology-for-Hass/main/examples/Metro%20Theme%20Thumbnail%203.png"/></td>
    <td>Revamp your More Info cards and various system UI screens to look extra clean and slick. <img alt="Systemwide Theming" src="https://raw.githubusercontent.com/Madelena/Metrology-for-Hass/main/examples/Metro%20Theme%20Thumbnail%204.png"/></td>
  </tr>
</table>

### Screenshots

|   |   |   |   |
|--- | --- | ---| ---|
| ![Red Theme (Light)](https://raw.githubusercontent.com/Madelena/Metrology-for-Hass/main/examples/HA%20Metrology%20-%20Color%20Themes%20-%20Red%20(Light).png) | ![Orange Theme (Light)](https://raw.githubusercontent.com/Madelena/Metrology-for-Hass/main/examples/HA%20Metrology%20-%20Color%20Themes%20-%20Orange%20(Light).png) | ![Green Theme (Light)](https://raw.githubusercontent.com/Madelena/Metrology-for-Hass/main/examples/HA%20Metrology%20-%20Color%20Themes%20-%20Green%20(Light).png) | ![Blue Theme (Light)](https://raw.githubusercontent.com/Madelena/Metrology-for-Hass/main/examples/HA%20Metrology%20-%20Color%20Themes%20-%20Blue%20(Light).png) |
| ![Red Theme (Dark)](https://raw.githubusercontent.com/Madelena/Metrology-for-Hass/main/examples/HA%20Metrology%20-%20Color%20Themes%20-%20Red%20(Dark).png) | ![Orange Theme (Dark)](https://raw.githubusercontent.com/Madelena/Metrology-for-Hass/main/examples/HA%20Metrology%20-%20Color%20Themes%20-%20Orange%20(Dark).png) | ![Green Theme (Dark)](https://raw.githubusercontent.com/Madelena/Metrology-for-Hass/main/examples/HA%20Metrology%20-%20Color%20Themes%20-%20Green%20(Dark).png) | ![Blue Theme (Dark)](https://raw.githubusercontent.com/Madelena/Metrology-for-Hass/main/examples/HA%20Metrology%20-%20Color%20Themes%20-%20Blue%20(Dark).png) |
| ![Device Example (Dark)](https://raw.githubusercontent.com/Madelena/Metrology-for-Hass/main/examples/HA%20Metrology%20-%20Device%20Example%20(Dark).png) Device Example | ![Device Example (Light)](https://raw.githubusercontent.com/Madelena/Metrology-for-Hass/main/examples/HA%20Metrology%20-%20Device%20Example%20(Light).png) Device Example | ![Binary Sensor Example (Dark)](https://raw.githubusercontent.com/Madelena/Metrology-for-Hass/main/examples/HA%20Metrology%20-%20More%20Info%20Box%20Example%20-%20Binary%20Sensor%20(Dark).png) Binary Sensor Example | ![Device Example (Dark)](https://raw.githubusercontent.com/Madelena/Metrology-for-Hass/main/examples/HA%20Metrology%20-%20More%20Info%20Box%20Example%20-%20Binary%20Sensor%20(Light).png) Binary Sensor Example | 
| ![Update (Dark)](https://raw.githubusercontent.com/Madelena/Metrology-for-Hass/main/examples/HA%20Metrology%20-%20More%20Info%20Box%20Example%20-%20Update%20(Dark).png) Update Example | ![Update (Light)](https://raw.githubusercontent.com/Madelena/Metrology-for-Hass/main/examples/HA%20Metrology%20-%20More%20Info%20Box%20Example%20-%20Update%20(Light).png) Update Example | ![Sensor Example (Dark)](https://raw.githubusercontent.com/Madelena/Metrology-for-Hass/main/examples/HA%20Metrology%20-%20More%20Info%20Box%20Example%20-%20Sensor%20(Dark).png) Sensor Example | ![Sensor Example (Dark)](https://raw.githubusercontent.com/Madelena/Metrology-for-Hass/main/examples/HA%20Metrology%20-%20More%20Info%20Box%20Example%20-%20Sensor%20(Light).png) Sensor Example | 
| ![Settings Example](https://raw.githubusercontent.com/Madelena/Metrology-for-Hass/main/examples/HA%20Metrology%20-%20Settings%20Example%20(Light).png) Settings Example | | | |
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

1. Create a new folder named `themes` under `/config`.
2. Copy [`metro.yaml`](/themes/metro.yaml) to `/config/themes`.
3. (Optional if you want Segoe UI on non-Windows devices) Copy [`style.css`](/www) and the `.ttf` font files to `/www`.
4. Restart Home Assistant to apply the changes.
5. Go to your Profile page, which is the button where your avatar is at the bottom left.
6. Under Themes, choose the color you like for the Metro themes.
7. Pick Auto, Light, or Dark Mode for the theme.

![Installation Instructions](https://raw.githubusercontent.com/Madelena/Metrology-for-Hass/main/examples/Installation%20Instructions.png)

Segoe UI font is optional if you are already using Windows. If you are not using Home Assistant, you can download the fonts [here](https://docs.microsoft.com/en-us/windows/apps/design/downloads/#fonts) and upload them along with style.css to your /config/www folder.

## Live Tile Templates

This is for advanced users only. If you don't know how to edit YAML, this will be rather difficult.

TBD. Includes button-card templates in the form of Live Tiles. Watch this repo for updates.

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





## Credits

![Creative Commons License](https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png)

This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-nc-sa/4.0/).

Additionally, I would appreciate proper credits back to me if redistributed or modified. That would help my livelihood since design is [my career](https://MadelenaMak.com).

The initial code was partially based on the [JuanMTech's AMOLED Theme](https://community.home-assistant.io/t/amoled-blue-theme-juanmtech/164458).
