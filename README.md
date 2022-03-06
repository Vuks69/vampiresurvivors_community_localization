# Vampire Survivors Community Localization Files

Partially updated for Vampire Survivors v0.3.0

Currently available community translations: PL, UK, TR, DE, EO, AR, HU, ZH-CN

## Official sources

Official Discord: https://discord.com/invite/vampire-survivors

Steam page: https://store.steampowered.com/app/1794680/Vampire_Survivors/

Official repository for community translation tools: https://github.com/Poncle/vampire-survivors-localisation

## Installation

Download all `.json` files and put them in `Vampire Survivors\resources\app\.webpack\renderer\assets\lang\`

To easily get to the game's base folder, go to your Steam Library, rightclick the game and select `Manage > Browse local files`

## Want to help?

You can fork this repository, update the relevant translations and open a PR, or post your own google spreadsheet/generated files in the `Localization` topic found on the [#modding](https://discord.com/channels/904353235006017556/937659884470693908) channel on the official discord.

In order to easily open a PR without having to copypaste your own translations between JSON files, you can:
* Create a Python script - get it [here](https://gist.github.com/Vuks69/71345df52392ace544d2f2d4ffd68474)
* Prepare the files like this:

```
/
├─ updater.py
├─ final/
└─ sources/
    ├─ base/
    │      achievementLang.json
    │      characterLang.json
    │      itemLang.json
    │      lang.json
    │      langKeys.json
    │      powerUpLang.json
    │      stageLang.json
    │      weaponLang.json
    ├─ pl/
    │      achievementLang.json
    │      characterLang.json
    │      itemLang.json
    │      lang.json
    │      langKeys.json
    │      powerUpLang.json
    │      stageLang.json
    └─     weaponLang.json
```

* `final` folder is where the resulting files will be written - this is what you need to commit for the Pull Request
* `base` - put the current JSON files from this repo in there!
* `pl` - rename this folder to your language's code (you can find it in any of the JSON files), and put your translated JSON files in here
* in the `updater.py` script, don't forget to change the `input_langs` variable to only contain your language's code! eg. `input_langs = ["pl"]`

When you open a PR with the above method, please attach the created `log.txt` file. It will help with catching any problems.

## Contributors
* PL/Polski:
  * WikiDev#1816 (@Wikizza)
  * RedHeadMaster#6618 (@RedHeadMaster)
  * Vuks#5767 (@Vuks69)
  * DavidGildour#3337
* UK/Українська:
  * Pilgrim#5341
* TR/Türkçe:
  * sicey9#0293
  * Mark Lindsay
* DE/Deutsch:
  * ReverseZoom#4923
* EO/Esperanto:
  * ᏕᏖᎩᎶᎥᎶᎧᏖᏂ ♡#7082
* AR/العربية
  * SoHyped#1111
* HU/Magyar
  * aronsz#3762
* FR/Français
  * Dimithreesome#4205
* zh-CN/简体中文
  * @XHXIAIEIN
