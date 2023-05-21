# System Metadata Files for ES-DE
This repo contains XML files that add system metadata variables for use in themes created for [ES-DE](https://es-de.org/)

The files leverage ES-DE variables to allow the values to be used in any theme agnostic of how the theme is structured.

It also includes a `_default.xml` that can be used as a temporary fallback for when new systems are added to ES-DE

Each file provides the following metadata variables:
- `systemDescription` - A description of the system
- `systemReleaseYear` - The year the system was released (when available)
- `systemReleaseDate` - The date the system was released in ISO 8601 (`YYYY-MM-DD`) format.  If only the month and year was known then the format is `YYYY-MM`.  If only the year was known then the format is `YYYY`.
- `systemReleaseDateFormated` - A formated version of the release date in `Month Day, Year` format.  If only the month and year was known then the format is `Month Year`.  If only the year was known then the format is `Year`.
- `systemHardwareType` - A value to represent the systems type (e.g. `Console`. `Portable`, `Computer`, etc...)
- `systemColor` - A hex value to represent a systems primary color (can be used for things like backgrounds or navigation highlights)
- `systemColorPalette1...4` - 4 different hex values to represent other colors that can be used for a system (useful for things like color bands)

## **Usage**
1. Download the latest release of this repo and place it in a dedicated folder in your theme.  
   - I recommend a dedicated folder like this: `/_inc/systems/metadata-global/` 
   - This approach will make it easier to update when changes are made.
2. Include a reference to files at the top of your root theme.xml file
   - As an example; I add the following includes in my themes:
   - `<include>./_inc/systems/metadata-global/_default.xml</include>` - default file for fallback use cases
   - `<include>./_inc/systems/metadata-global/${system.theme}.xml</include>` - the system specific xml file
3. Reference a value using the variable names listed above
   - For example if you wanted to add system specific colors to a UI element you would refernece `${systemColor}` for that value
   
## **Contributions**
- If you see any existing values that should be updated with more accurate data; please submit an issue or PR to this repo.  Make sure to include the system, specific change and the reason for the change in your request.
- If you have an idea for a new variable to add; please submitt an issue to this repo with details of the variable and what it could be used for.

## **Examples**
Here are some examples of this repo being used in ES-DE themes:
| [Colorful (Revisited)](https://github.com/anthonycaccese/colorful-revisited-es-de) | [Colorful (Simplified)](https://github.com/anthonycaccese/colorful-simplified-es-de) |
| :---: | :---: |
| <img src="https://user-images.githubusercontent.com/1454947/224544826-8067eb32-b4d2-41ee-8cce-19c4794ab05f.png"> | <img src="https://user-images.githubusercontent.com/1454947/224544816-be13c05e-b322-4d6c-8289-efc20d7f97bd.png"> |
| [Chicuelo (Revisited](https://github.com/anthonycaccese/chicuelo-revisited-es-de) | [Epic Noir (Revisited)](https://github.com/anthonycaccese/epic-noir-revisited-es-de) |
| <img src="https://user-images.githubusercontent.com/1454947/224714965-ad168dc9-f921-493f-a620-cefbf318cc61.png"> | <img src="https://user-images.githubusercontent.com/1454947/224715009-6d5c60bd-df04-40e0-88a2-32f5a45b8e8a.png"> |
| [Retrofix (Revisited)](https://github.com/anthonycaccese/retrofix-revisited-es-de) |
| <img src="https://user-images.githubusercontent.com/1454947/224544794-ced156ff-dd35-47ea-b6c9-fb6f83db95c0.png"> |

## **Credits**
* Some descriptions, release dates & manufacturer details were sourced from the wikipedia entries for each system
* Some descriptions were sourced from [ckau-book](https://github.com/CkauNui/ckau-book/tree/master)
* Some release date and manufacturer details were sourced from the [Launchbox](https://gamesdb.launchbox-app.com/) platforms list
* System colors were sourced from the great work done by [viking](https://forums.launchbox-app.com/profile/70421-viking/) from their work on the [Colorful](https://forums.launchbox-app.com/files/file/2081-colorful-bigbox-theme) theme for Launchbox and [@rogs123](https://github.com/rogs123) from their work on the [NSO Menu](https://github.com/anthonycaccese/nso-menu-interpreted-es-de) theme for ES-DE

## **License**
Creative Commons CC-BY-NC-SA - https://creativecommons.org/licenses/by-nc-sa/2.0/
You are free to share and adapt these files as long as you provide attribution back as well share any updates you make under the same licence terms.