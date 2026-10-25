---
title: "XpsOptions"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "プロジェクトページを XPS にレンダリングする際の追加オプションを指定できます。"
type: docs
weight: 369
url: /ja/java/com.aspose.tasks/xpsoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.ICloneableSaveOptions
```
public class XpsOptions extends SaveOptions implements ICloneableSaveOptions
```

プロジェクトページを XPS にレンダリングする際の追加オプションを指定できます。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [XpsOptions()](#XpsOptions--) | 新しい [XpsOptions](../../com.aspose.tasks/xpsoptions) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getRenderMetafileAsBitmap()](#getRenderMetafileAsBitmap--) | メタファイルをビットマップとしてレンダリングすべきかどうかを示す値を取得します。 |
| [setRenderMetafileAsBitmap(boolean value)](#setRenderMetafileAsBitmap-boolean-) | メタファイルをビットマップとしてレンダリングすべきかどうかを示す値を設定します。 |
### XpsOptions() {#XpsOptions--}
```
public XpsOptions()
```


新しい [XpsOptions](../../com.aspose.tasks/xpsoptions) クラスのインスタンスを初期化します。

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public final void copyOutputPropertiesFrom(SaveOptions source)
```


内部使用のために予約されています。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| source | [SaveOptions](../../com.aspose.tasks/saveoptions) | \{@inheritDoc\} |

### deepClone() {#deepClone--}
```
public final SaveOptions deepClone()
```


内部使用のために予約されています。

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getRenderMetafileAsBitmap() {#getRenderMetafileAsBitmap--}
```
public final boolean getRenderMetafileAsBitmap()
```


メタファイルをビットマップとしてレンダリングすべきかどうかを示す値を取得します。

**Returns:**
boolean - メタファイルをビットマップとしてレンダリングすべきかどうかを示す値。
### setRenderMetafileAsBitmap(boolean value) {#setRenderMetafileAsBitmap-boolean-}
```
public final void setRenderMetafileAsBitmap(boolean value)
```


メタファイルをビットマップとしてレンダリングすべきかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | メタファイルをビットマップとしてレンダリングすべきかどうかを示す値。 |

