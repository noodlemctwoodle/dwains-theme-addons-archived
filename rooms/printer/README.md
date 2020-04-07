# Printer Add-on




### Installation
- Install [bar-card](https://github.com/custom-cards/bar-card) from [HACS](https://hacs.xyz).
- Configure your `custom_resources.yaml` file in `<config dir>/dwains-theme/resources` with the config below.
- Copy the files `page.yaml` and `button.yaml` to your `<config dir>/dwains-theme/addons/rooms/<your room>/printer` directory.
- Configure your `rooms.yaml` file in `<config dir>/dwains-theme/configs` with config below.
- Reload theme configuration at Theme settings.


### Usage
To use this add-on in your Dwains Theme, add the following to your `custom_resources.yaml` and `rooms.yaml` file:
```yaml
# Example custom_resources.yaml entry
- url: /hacsfiles/bar-card/bar-card.js
  type: js
```

```yaml
# Example rooms.yaml entry
  - name: Office
    addons:
      - name: Printer
        icon: fas:print
        path: 'dwains-theme/addons/rooms/office/printer/page.yaml'
        button_path: 'dwains-theme/addons/rooms/office/printer/button.yaml'
        data:
          entity: sensor.hp_printer_status
```

### Screenshots
**Light theme:**<br>
![mobile-light](https://github.com/Klumpke/dwains-theme-addons/blob/master/rooms/printer/.github/screenshots/mobile-light.png "Mobile Light")

![tablet-light](https://github.com/Klumpke/dwains-theme-addons/blob/master/rooms/printer/.github/screenshots/tablet-light.png "Tablet Light")

**Dark theme:**<br>
![mobile-dark](https://github.com/Klumpke/dwains-theme-addons/blob/master/rooms/printer/.github/screenshots/mobile-dark.png "Mobile Dark")

![tablet-dark](https://github.com/Klumpke/dwains-theme-addons/blob/master/rooms/printer/.github/screenshots/tablet-dark.png "Tablet Dark")


### Changelog
#### 1.0.0
- First release