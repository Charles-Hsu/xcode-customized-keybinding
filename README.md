xcode-customized-keybinding
===========================
紀錄一下 Xcode 的 Keybinding 的做法

1. 打開路徑 /Applications/Xcode.app/Contents/Frameworks/IDEKit.framework/Versions/A/Resources 下的 IDETextKeyBindingSet.plist 檔案, 加入幾行 xml 的定義. 不過, 我用 sublime 加了之後, Xcode 卻說格式不合

```
chia@mac1234 Resources% ls -l IDETex*
-rw-r--r--  1 root  wheel  15176 Nov  3 08:05 IDETextAttributesBackgroundColorGlyph.opacity
-rw-r--r--  1 root  wheel   3035 Nov  3 08:05 IDETextAttributesBackgroundColorGlyph.pdf
-rw-rw-rw-@ 1 chia  wheel  11333 Nov 24 16:27 IDETextKeyBindingSet.plist
chia@mac1234 Resources% pwd
/Applications/Xcode.app/Contents/Frameworks/IDEKit.framework/Versions/A/Resources

```

2. 所以乾脆把改好的檔案存到 github 來, 下次要用到時, 直接覆蓋過去就好了
3. Restart Xcode, Preference/Key Binding, 選 Customized, 在其中設定 Delete Current Line, Insert New Line Below, Insert New Line Above, Duplicate Current Line 的組合鍵

[畫面如下:](https://github.com/Charles-Hsu/xcode-customized-keybinding/blob/master/xcode-key-bindings-config.png)



