# 作用

以气泡方式显示文档内容 ，同时提供自定义背景，支持图片，视频及动态网页。

# 使用方法

1. 打开插件
2. 将你希望使用的壁纸文件放入你思源笔记的工作空间文件夹 `\data\public\backgrounds\` 内。
3. 打开设置界面，使用默认快捷键`ctrl+shift+F9`，或者在思源主界面右上角点击此插件的图标 ![toolbaricon](https://github.com/user-attachments/assets/2f74322e-abe5-4f21-b6df-cede7334c489)
4. 点击 `重新加载资源文件` 按钮以重新加载壁纸文件，点击播放下一个切换壁纸。
5. 可以使用快捷键`ctrl+shift+F8`快速切换壁纸。

# 预览

![preview](https://github.com/user-attachments/assets/c2b8598a-2b15-49fc-a19d-f3d24aabbe49)

![preview2](https://github.com/user-attachments/assets/617188b4-7dc0-4c20-9fb4-3b83df16b32e)

![设置](https://github.com/user-attachments/assets/605a2921-bae7-4038-9bce-56763e830892)

# 资源文件使用说明

![resource folder](https://github.com/user-attachments/assets/63217ac3-561b-43fb-a342-b0d765fe733f)

`v://Siyuan` 是我的思源笔记工作空间，假如你的在其他盘符，那就去对应盘符。假如该文件夹不存在，插件第一次打开的时候会自动创建，并放入两个动态网页壁纸`space`和`statrs`。

## 图片和视频

支持大多数格式，放入该文件夹内就可以。

## 动态网页壁纸

必须放在子文件夹内，文件夹的名称会被识别为壁纸名称，其中`index.html`作为壁纸主体会被加载。

# 兼容性

## 支持的主题

以下是我在使用的主题，所以确定能适配

1. 默认主题
2. pink-room
3. Dark+
4. vert

## 其他主题

壁纸的工作原理是在页面的底层添加了一个画布用来显示壁纸。假如你使用的其他主题,壁纸不能显示的时候，你可以使用`开发者工具`找到叠加在上层的元素。将对应的css代码添加到`代码片段`中应用。

比如当你使用主题Savor时，在你的`代码片段`中添加这部分并启用。
`
#toolbar + .fn__flex {
    background-color: transparent;
}
`

# 其他

1. 在设置界面双击壁纸名称可以直接切换。
2. 播放筛选器在关闭设置界面时才会刷新，之后使用快捷键切换就好。
3. 优秀的动态壁纸推荐wallpaper engine找找。