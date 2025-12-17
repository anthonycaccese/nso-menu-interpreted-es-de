# NSO Menu Interpreted (ES-DE Version)

A simple theme for the version of EmulationStation used in [ES-DE](https://es-de.org/)  The design is inspired by the Menu UI from [Nintendo Switch Online](https://en.wikipedia.org/wiki/Nintendo_Switch_Online).  It includes a custom grid view built to match the cover artwork for each supported system.

This theme was created in collaboration with [@rogs123](https://github.com/rogs123)

![preview](https://github.com/anthonycaccese/nso-menu-interpreted-es-de/assets/1454947/02db0180-f21f-49d4-9d63-2a57c68511f1)

## **Preview**

| System View | Gamelist View |
|----|----|
| ![Screenshot 2023-11-20 at 10 31 36 AM](https://github.com/anthonycaccese/nso-menu-interpreted-es-de/assets/1454947/cf36956f-136b-4fd3-b2fd-7fe4cafc1a6c) | ![Screenshot 2023-11-20 at 10 31 44 AM](https://github.com/anthonycaccese/nso-menu-interpreted-es-de/assets/1454947/bb423406-9077-4dfd-bcd7-51ede5a49411) |


## **Configuration Options**

- The theme has a simple set of options that can be changed directly from the UI Settings menu of ES-DE 
- `Theme Aspect Ratio` - sets the aspect ratio the theme will render at. If needed, this should be changed to match the aspect ratio of your screen.
   - 16:9, 16:10, 8:7, 1:1 and 4:3 aspect ratios are supported
- `Color Scheme` - sets the images displayed on system view and colors like the menu bar background and grid selector. There are a few built in options and a custom option which allows you to set your own values for some properties.  Instructions for using custom are in the `Customizations` section below.

## Customizations

A custom color scheme lets you modify some theme options while also allowing you to continue to get updates from the theme downloader.

1. In the resources folder you will find a template file called `customizations.xml`

2. Make a folder named theme-customizations and place a copy of the customizations.xml file inside that folder. The folder structure should look like this when you are done:

   ```
   /ES-DE/themes/nso-menu-interpreted-es-de/theme-customizations/customizations.xml
   ```

   For the Android theme downloader version this would be:

   ```
   /Android/data/org.es_de.frontend/files/themes/nso-menu-interpreted-es-de/theme-customizations/customizations.xml
   ```

4. Edit the properties in customizations.xml to make theme customizations. There are comments within the template that explain each property. If you have questions just ask.

5. Set the Theme Color Scheme in ES-DE's UI Settings menu to `Custom` and you should see your customizations. If you see an error check that the paths discussed above are correct and then check that the values you added for each property are correct and well formatted.

## **Acknowledgments**

* Most system images were sourced from the excellent work done by “viking” and many other contributors to the COLORFUL platform video set [here](https://forums.launchbox-app.com/files/file/1958-colorful-platform-video-set/).
* Some controller artwork ws sourced from the excellent work by [Pineapple_Graphics](https://archive.org/details/full-color-pngs)
* Some controller artwork was sourced from the excellent work by [RickyRomero](https://dribbble.com/RickyRomero) via their work for OpenEMU
* The base folder icon that was used to create the All Games, Favorites, Last Played and Custom Collections images was sourced from [Rick Patrick](https://www.softicons.com/designers/rick-patrick)

## **License**

Creative Commons CC-BY-NC-SA - https://creativecommons.org/licenses/by-nc-sa/2.0/
You are free to share and adapt this theme as long as you provide attribution back to me (and the above Acknowledgments) as well share any updates you make under the same licence terms.  This theme (and all of its contained assets) are not to be used for commercial purposes.
