
# Function

Display document content in floating bubbles while providing customizable backgrounds, supporting images, videos, and dynamic webpages.

# Usage

1. Open the plugin  
2. Place wallpaper files you wish to use in your Siyuan Note workspace folder `\data\public\backgrounds\`.  
3. Open settings using the default shortcut `ctrl+shift+F9`, or click the plugin icon in the top-right corner of the Siyuan interface: ![sc_2025-04-08_12-32-06](assets/sc_2025-04-08_12-32-06-20250408123210-fwnp8uv.jpg)  
4. Click the `Reload Resource Files` button to refresh wallpaper files. Click "Play Next" to switch wallpapers. 
5. You can also use the shortcut key `Ctrl+Shift+F8` to quickly switch wallpapers.

# Preview

![sc_2025-04-08_12-18-23](assets/sc_2025-04-08_12-18-23-20250408121835-jl41rzr.jpg)![sc_2025-04-08_12-33-55](assets/sc_2025-04-08_12-33-55-20250408123359-zc1wto6.jpg)

# Resource File Instructions

![sc_2025-04-08_12-48-38](assets/sc_2025-04-08_12-48-38-20250408124845-cuz7242.jpg)

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