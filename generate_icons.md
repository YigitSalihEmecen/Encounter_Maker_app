# Generate App Icons

To generate proper launcher icons for the app, follow these steps:

## Using Android Studio (Recommended)

1. Open the project in Android Studio
2. Right-click on the `app` folder in the Project view
3. Select **New > Image Asset**
4. Choose **Launcher Icons (Adaptive and Legacy)**
5. Configure your icon:
   - **Foreground Layer**: You can use the vector drawable we created or upload your own image
   - **Background Layer**: Use the background color `#8B4513` (brown) or the vector drawable
   - **Legacy Icon**: Generate for older Android versions
6. Click **Next** and then **Finish**

This will automatically generate all required icon sizes for different screen densities.

## Manual Icon Sizes Needed

If creating manually, you need these sizes:

- **mdpi**: 48x48 px
- **hdpi**: 72x72 px  
- **xhdpi**: 96x96 px
- **xxhdpi**: 144x144 px
- **xxxhdpi**: 192x192 px

Place them in the corresponding `mipmap-*` folders:
- `app/src/main/res/mipmap-mdpi/ic_launcher.png`
- `app/src/main/res/mipmap-hdpi/ic_launcher.png`
- `app/src/main/res/mipmap-xhdpi/ic_launcher.png`
- `app/src/main/res/mipmap-xxhdpi/ic_launcher.png`
- `app/src/main/res/mipmap-xxxhdpi/ic_launcher.png`

Also create round versions with `_round` suffix for each density.

## Icon Design Suggestions

For the DnD Initiative Tracker app, consider:
- D&D themed elements (dice, dragons, scrolls)
- Initiative/turn order symbols
- Fantasy RPG aesthetics
- Use the app's color scheme: brown (`#8B4513`) and gold (`#D4AF37`) 