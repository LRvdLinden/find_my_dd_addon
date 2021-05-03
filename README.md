<h1 align="center">Find My - Dwains Dashboard Add-on (more_page)</h1> 


<p align="center">
  <a href="https://dwainscheeren.github.io/dwains-lovelace-dashboard/">
    <img src="https://img.shields.io/badge/Dwains%20Dashboard-Default-299ec2.svg" />
  </a>
  <a href="https://github.com/custom-components/hacs">
    <img src="https://img.shields.io/badge/HACS-Default-orange.svg" />
  </a>
  <a href="https://github.com/LRvdLinden/find_my_dd_addon">
    <img src="https://img.shields.io/github/v/release/LRvdLinden/weather_dd_addon" />
  </a>
    <a href="https://github.com/LRvdLinden/">
    <img src="https://img.shields.io/github/followers/LRvdLinden?style=social" />
  </a>
    </a>
    <a href="https://discord.gg/7yt64uX">
    <img src="https://img.shields.io/discord/688401603811999885" />
  </a>
</p>
<p align="center">Find My in Home Assistant Dwains Dashboard.</p>


<p align="center">Created by <a href="https://github.com/LRvdLinden">Léon van der Linden</a>
</p> 


<p align="center">
  <img src="https://cdn.wccftech.com/wp-content/uploads/2021/03/Find-My-Using-Siri-HomePod.png" />
</p>



## Prerequisite ⚙️
---
- Make sure you have installed the lovelace [fold-entity-row](https://github.com/thomasloven/lovelace-fold-entity-row), [fontawesome icons](https://github.com/thomasloven/hass-fontawesome), [Cupertino Icons](https://github.com/menahishayan/HomeAssistant-Cupertino-Icons), [Button Card](https://github.com/custom-cards/button-card) and the integration [Neerslag app](https://github.com/aex351/home-assistant-neerslag-app). This can be done manually or directly via hacs

<img width="618" alt="image" src="https://user-images.githubusercontent.com/77990847/114733529-b6ca1a00-9d43-11eb-876a-6f4beda466ec.png">


## Installation Add-on ⚙️
---
- Copy the `find_my` folder in to the `dwains-dashboard/addons/more_page` directory.
- Open your `more_page.yaml` file in `dwains-dashboard/configs` and add the following;
```yaml
  - name: Find My
    main_menu: 'true' #Show this addon in the main navigation bar!
    icon: mdi:radar
    path: 'dwains-dashboard/addons/more_page/find_my/page.yaml'
```
- Reload the theme configuration via Theme Settings

## Add more cards
---
- If some `sensors` not showing after this manual, please add the correct `sensor` to monitor
- The dashboard will refresh every 10 minutes. When you want to skip this, delete the code between line 66 till 69
```yaml
 - cards:
   Refresh: null
   type: 'custom:auto-reload-card'
   delay_in_minute: 10
```

## Result
---
![image](https://user-images.githubusercontent.com/77990847/116847119-2e27f680-abea-11eb-8eaf-02a91e623a1b.png)

![image](https://user-images.githubusercontent.com/77990847/116847363-ae4e5c00-abea-11eb-86ee-27dd2e964094.png)



---
Enjoy my card? Help me out for a couple of :beers: or a :coffee:!

[![coffee](https://www.buymeacoffee.com/assets/img/custom_images/black_img.png)](https://www.buymeacoffee.com/LRvdLinden)
