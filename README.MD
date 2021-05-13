# fcitx5 九八五笔码表

## 适用范围

码表为`dict`格式，适用于`fcitx5`。  

## 感谢
感谢码表整理者**yanhuacuo**大佬，码表githup链接[https://github.com/yanhuacuo/98wubi-tables](https://github.com/yanhuacuo/98wubi-tables)  
感谢 fcitx5 的开发者, fcitx5 开发地址:[https://github.com/fcitx/fcitx5](https://github.com/fcitx/fcitx5)  
其实我要吐槽一下，虽然提供了码表制作工具`libime_tabledict`，可是使用说明几乎没有，对文本的要求也没写明，从`txt`转换成`dict`时**segmentation fault**出现了好几次，差点我就放弃制作了。  

## 使用方法  
1. 首先当然需要安装`fcitx5`，推荐同时安装`fcitx5-chinese-addons`。  
2. 然后将码表文件拷贝到`libime`目录  
```sh
sudo cp wb98.main.dict /usr/share/libime/
```
3. 将配置文件拷贝到`fcitx5`下的输入法目录
```sh
sudo cp wb98.conf  /usr/share/fcitx5/inputmethod/
```
4. 重启`fcitx5`输入法  

  然后在`fcitx5` 配置菜单中添加**五笔九八**输入法即可。

5. 附赠一个输入法图标  
  ![](org.fcitx.Fcitx5.fcitx-wb98.png)  
  `Debian + KDE`系统，可将此图更名为`org.fcitx.Fcitx5.fcitx-wb98.png`，拷贝到`/usr/share/icons/hicolor/48x48/apps/`目录下，然后在`wb98.conf`配置文件中修改`Icon=fcitx-wb98`，重启输入法即可刷新托盘图标。
