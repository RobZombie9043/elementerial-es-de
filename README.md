# elementerial-es-de
A port of the [Elementerial](https://github.com/mluizvitor/es-theme-elementerial) theme by [mluizvitor](https://github.com/mluizvitor/es-theme-elementerial/commits?author=mluizvitor) for ES-DE. It's based on Android TV's interface using some principles from Material Design with the addition of ElementaryOS color palette.

## **Preview**
| System View (Classic) | System View (Modern) | 
|----|----|
| ![Screenshot_20240929-230241](https://github.com/user-attachments/assets/c28a4787-44a5-4605-8373-fc6079dcfbe3) | ![Screenshot_20240929-230118](https://github.com/user-attachments/assets/92087554-278e-42b4-ad88-83f971dfc36e) |

| List: Basic View | List: Video View | List: Detailed View |
|----|----|----|
| ![Screenshot_20240929-230445](https://github.com/user-attachments/assets/dbf8356b-774a-4ad0-84f2-5ad1f9bd4a01) | ![Screenshot_20240929-230518](https://github.com/user-attachments/assets/4671d6e8-44fc-4518-ac63-6dee5c353738) | ![Screenshot_20240919-164040](https://github.com/user-attachments/assets/0a716055-46ea-403d-9c83-ecc2cfdc630f) |

| Elementflix View | Grid View (Small) | Grid View (Large) |
|----|----|----|
| ![Screenshot_20240919-163316](https://github.com/user-attachments/assets/db111aab-a1e3-4bbc-905c-265eef1f0609) | ![Screenshot_20240929-230652](https://github.com/user-attachments/assets/09e5f776-a45a-4710-a868-44a9f5c0a246) | ![Screenshot_20240929-230605](https://github.com/user-attachments/assets/d71380f4-53cb-42d9-b886-4628a90ee846) |

## **Changes made**
- Any changes from the original theme were largely unintentional or due to differences in theme engines
- Additional aspect ratios created
- Due to no composite element support, the grid view variants were modified to suit box art
- System logos for additional systems supported by ES-DE were created by me 

## **Configuration Options**

- This theme has a simple set of options that can be changed directly from the UI Settings menu of ES-DE
  
- `Theme Variant` - sets the theme variant adjusting the gamelist view. Each variant has a Modern, Classic or Video option which adjusts the background Artwork used in the theme
   - `List: Basic View`
   - `List: Video View`
   - `List: Detailed View`
   - `Elementflix View`
   - `Grid View (Small)`
   - `Grid View (Large)`

 - `Theme Color Scheme` - sets the theme color scheme adjusting the background image color. Each color scheme has a Light and Dark variant.
   - `Strawberry`
   - `Orange`
   - `Banana`
   - `Lime`
   - `Mint`
   - `Blueberry`
   - `Grape`
   - `Bubblegum`
   - `Cocoa`
   - `Slate`
   - `SNES`
   - `Gameboy`
   - `Pikachu Edition`
   - `Red Fruits`
     
- `Font Size` - enables you to change the size of the fonts displayed in the theme.
   - `Small`
   - `Medium`
   - `Large`
     
- `Theme Aspect Ratio` - sets the aspect ratio the theme will render at. If needed, this can be changed to match the aspect ratio of your screen (though it should happen automatically).
   - `16:9`
   - `16:10`
   - `4:3`
   - `1:1`
   - `3:2`
   - `5:4`
   - `19.5:9`
   - `21:9`

## **Theme Customization Options**
- Custom theme artwork can be provided for use in the theme. Custom artwork will be shown for any systems that are added and will fallback to the included theme artwork where no images are provided.
1.  Create a folder named `theme-customizations` within the main elementerial-es-de theme folder
2.  To add custom artwork to:
    - the modern artwork set - create a subfolder named artwork (modern) <br>
      `/ES-DE/themes/elementerial-es-de/theme-customizations/artwork (modern)/`
    - the classic artwork set - create a subfolder named artwork (classic) <br>
      `/ES-DE/themes/elementerial-es-de/theme-customizations/artwork (classic)/`
3. Add your custom artwork in .webp format to to this folder named `${system.theme}.webp`. For example if you wanted to override the artwork for `snes` you would create an image called `snes.webp` in the chosen artwork folder.
4. [Optional] To modify the y-axis positioning of the artwork displayed:
   - Create a folder named `metadata-custom` within the `theme-customizations` folder
   - Create a `${system.theme}.xml` file
   - Add the following code and adjust the crop position to suit, where 0 means align on top and 1 means align at the bottom. Any arbitrary floating point values between 0 and 1 can be used for granular positioning.
   ```
   <theme>
     <variables>
       <classicCropPos>0.5</classicCropPos>
       <modernCropPos>0.5</modernCropPos>
     </variables>
   </theme>
   ```

- The original theme artwork can be found [here](https://www.mediafire.com/file/cl5xozj31ztnyyt/theme-customizations.zip/file) and can be used by unzipping the included theme-customization folder to the theme folder.

## **Acknowledgements**
- Based on original [Elementerial](https://github.com/mluizvitor/es-theme-elementerial) theme by [mluizvitor](https://github.com/mluizvitor/es-theme-elementerial/commits?author=mluizvitor)
- [Inter Font](https://github.com/rsms/inter) by [rsms](https://github.com/rsms)
