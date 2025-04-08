
# Function

Display document content in floating bubbles while providing customizable backgrounds, supporting images, videos, and dynamic webpages.

# Usage

1. Open the plugin  
2. Place wallpaper files you wish to use in your Siyuan Note workspace folder `\data\public\backgrounds\`.  
3. Open settings using the default shortcut `ctrl+shift+F9`, or click the plugin icon in the top-right corner of the Siyuan interface: ![toolbaricon](https://github.com/user-attachments/assets/2f74322e-abe5-4f21-b6df-cede7334c489)

4. Click the `Reload Resource Files` button to refresh wallpaper files. Click "Play Next" to switch wallpapers. 
5. You can also use the shortcut key `Ctrl+Shift+F8` to quickly switch wallpapers.

# Preview

![preview](https://github.com/user-attachments/assets/c2b8598a-2b15-49fc-a19d-f3d24aabbe49)

![](https://github.com/user-attachments/assets/5f2dc064-b271-4211-85a2-1aead3211b20)


# Resource File Instructions

![resource folder](https://github.com/user-attachments/assets/ab28d889-abfe-4036-b9d5-2fd06d6bbec1)

`v://Siyuan` is my Siyuan Note workspace. If yours is on a different site, navigate to the corresponding drive. If the folder doesn’t exist, the plugin will automatically create it on first launch and add two dynamic webpage wallpapers: `space` and `stars`.

## Images & Videos

Supports most formats; simply place them in this folder.

## Dynamic Webpage Wallpapers

Must be placed in subfolders. The subfolder name will be recognized as the wallpaper name, and `index.html` within it will be loaded as the main content.

# Compatibility

## Supported Themes

The following themes have been tested and verified to be compatible:

1. Default Theme
2. pink-room
3. Dark+
4. vert

## Other Themes

The wallpaper implementation works by adding a canvas layer at the bottom of the page to display wallpapers. If your theme prevents the wallpaper from showing, use **Developer Tools** to identify elements overlaying the canvas layer. Add corresponding CSS code to your **Code Snippet** configuration to fix compatibility issues.

For example, when using the **Savor** theme, add and enable this code in your **Code Snippet**:
```
#toolbar + .fn__flex {
    background-color: transparent;
}
```

# Others  

1. Double-click the wallpaper name in the settings interface to switch directly.  
2. The play filter refreshes only when the settings interface is closed; use hotkeys to switch afterward.  
3. For excellent dynamic wallpapers, we recommend looking for them in Wallpaper Engine.
