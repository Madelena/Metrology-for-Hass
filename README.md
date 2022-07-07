![Collage of Screenshots showing the Metro theme in light and dark modes](https://user-images.githubusercontent.com/4341881/177691320-80597b03-cbac-434e-8242-7101cf80c6d0.png)

# Metrology for Home Assistant

Metrology is a practical series of app customizations and redesigns aimed at bringing a bold, clear, and consistent user experience to [various Windows and Android apps](https://github.com/Madelena?tab=repositories&q=Metrology). Its design language is based on [Metro](https://en.wikipedia.org/wiki/Metro_(design_language)) and [Fluent](https://www.microsoft.com/design/fluent/) design systems pioneered by Microsoft Design since the 2010s.

[Home Assistant](https://www.home-assistant.io/) is an open source home automation server that integrates nearly 2000 existing IoT services into one powerful, private, and unified user interface. It is perfect to run on a Raspberry Pi or a local server.

Here is a collection of themes, tweaks, and template buttons to make your Home Assistant look bold, modern, and clean.

**Discuss this theme on [Home Assistant Community](https://community.home-assistant.io/t/metrology-metro-fluent-windows-themes-for-home-assistant/419530) or [Reddit](https://www.reddit.com/r/homeassistant/comments/ui1uga/theme_metrology_metro_fluent_windows_themes_for/).**

To check out what this theme is capable of, check out my [Home Assistant config](https://github.com/Madelena/hass-config-public).

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/madelena)

**✨ Thank you @legovaer and @pbohannon for your generous support! ✨**

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
    <td>Display your home automation status with distinct and bold typography using Segoe UI or Segoe UI Variable fonts. <img alt="Typography" src="https://user-images.githubusercontent.com/4341881/177691335-311cec05-ee60-4937-a70c-d1b313609da5.png"/></td>
    <td>Use Light and Dark Modes natively. Dark Mode has a true black background great for AMOLED screens. <img alt="Light and Dark Modes" src="https://user-images.githubusercontent.com/4341881/177691336-ba4a0aa4-daff-44af-8ed5-9661367e460b.png"/></td>
  </tr>
  <tr width="50%">
    <td>Switch between 4 color themes. Also adding new themes is relatively easy thanks to YAML Anchors. <img alt="Color Themes" src="https://user-images.githubusercontent.com/4341881/177691338-82039962-61a9-4b4a-a366-5ae90d932c2f.png"/></td>
    <td>Revamp your More Info cards and various system UI screens to look extra clean and slick. <img alt="Systemwide Theming" src="https://user-images.githubusercontent.com/4341881/177691339-a91d58bf-dc01-4f1e-b35f-7478b4dafe61.png"/></td>
  </tr>
</table>

### Screenshots

|   |   |   |   |
|--- | --- | ---| ---|
| ![Red Theme (Light)](https://user-images.githubusercontent.com/4341881/177691313-4f6bf40d-9a05-4636-b08f-d59ca16cc42e.png) | ![Orange Theme (Light)](https://user-images.githubusercontent.com/4341881/177691311-ffab9423-6173-4165-ba28-c5ddacf1a347.png) | ![Green Theme (Light)](https://user-images.githubusercontent.com/4341881/177691308-e4515097-e21b-4b51-a7dd-abf07e2a4f30.png) | ![Blue Theme (Light)](https://user-images.githubusercontent.com/4341881/177691303-925e09ef-36df-46cc-9adb-947498371356.png) |
| ![Red Theme (Dark)](https://user-images.githubusercontent.com/4341881/177691313-4f6bf40d-9a05-4636-b08f-d59ca16cc42e.png) | ![Orange Theme (Dark)](https://user-images.githubusercontent.com/4341881/177691310-ad00da0a-ff8d-425b-8745-f9daab17b7ee.png) | ![Green Theme (Dark)](https://user-images.githubusercontent.com/4341881/177691307-5c214876-20e7-4126-92a9-d919ab4f6e26.png) | ![Blue Theme (Dark)](https://user-images.githubusercontent.com/4341881/177691302-43771ae0-4ca2-4147-8df8-844f884caddb.png) |
| ![Device Example (Dark)](https://user-images.githubusercontent.com/4341881/177691318-db533182-101d-466d-9252-8fff32ac3fad.png) Device Example | ![Device Example (Light)](https://user-images.githubusercontent.com/4341881/177691319-96d9bcf7-f1cc-44c6-8801-0686d7d8b328.png) Device Example | ![Binary Sensor Example (Dark)](https://user-images.githubusercontent.com/4341881/177691322-9b8cb693-94b1-48a6-8a2b-fe9350e31100.png) Binary Sensor Example | ![Binary Sensor Example (Light)](https://user-images.githubusercontent.com/4341881/177691323-4470bda0-0946-413e-bfbd-90ebadebdd67.png) Binary Sensor Example | 
| ![Update (Dark)](https://user-images.githubusercontent.com/4341881/177691330-ff03bd31-1985-43a5-ac56-74c703eb7a46.png) Update Example | ![Update (Light)](https://user-images.githubusercontent.com/4341881/177691331-7de1aa64-9f41-463e-a063-ccfdcea7beed.png) Update Example | ![Sensor Example (Dark)](https://user-images.githubusercontent.com/4341881/177691327-92fdad19-b4f9-46bd-979b-188790ca0f9e.png) Sensor Example | ![Sensor Example (Dark)](https://user-images.githubusercontent.com/4341881/177691329-5022abd5-442d-406d-8332-99a3937a880c.png) Sensor Example | 
| ![Settings Example](https://user-images.githubusercontent.com/4341881/177691332-3b69d8d9-d85d-4506-8e11-6404c9451d8d.png) Settings Example | | | |
| | | |

### How to Install the Theme

If you have HACS, you probably already know what you are doing. You can search for this theme and install it there. If you don't have HACS, here are the steps:

#### Prerequisites

- Some way to upload files to your HA server, e.g. Visual Studio Code or Samba add-ons
- card-mod

#### Installation

1. If you are new to Home Assistant and its themes, you first need to add this in your configuration.yaml file:
  ```yaml
  frontend:
    themes: !include_dir_merge_named themes
  ```
2. Create a new folder named `themes` under `/config`.
3. Copy [`metro.yaml`](/themes/metro.yaml) to `/config/themes`.
4. (Optional if you want Segoe UI on non-Windows devices) Copy [`style.css`](/www) and the `.ttf` font files in the `/www` folder to `/config/www`.
  - If you are using the Lovelace Dashboard not in YAML mode, go to your Home Assistant Settings -> Dashboards -> Resources and then add `/local/style.css` as a Stylesheet.
    (Note: It might look strange that you had copied the files to `/www` but here you typed `/local`, but HA will handle the path redirection for you so no worries.)
  - If you are using it in YAML mode, add the following to your lovelace resources section:
    ```yaml
      lovelace:
        mode: yaml
        resources:
          - url: /local/style.css
            type: css
    ```
5. Restart Home Assistant to apply the changes. Once restarted, go to your Profile page, which is the button where your avatar is at the bottom left.

![Installation Instructions](https://user-images.githubusercontent.com/4341881/177691334-56654b34-b594-4f60-a606-f56ea1591397.png)

6. Under Themes, choose the color you like for the Metro themes.
7. Pick Auto, Light, or Dark Mode for the theme.

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
