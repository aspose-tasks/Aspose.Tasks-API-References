---
title: "FontResolveEventArgs"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "フォントが解決されたときに呼び出されるコールバックの引数を提供します。"
type: docs
weight: 99
url: /ja/java/com.aspose.tasks/fontresolveeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public final class FontResolveEventArgs extends System.EventArgs
```

フォントが解決されたときに呼び出されるコールバックの引数を提供します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getRequestedFontName()](#getRequestedFontName--) | 要求されたフォントの名前を取得します。 |
| [getResolvedFontName()](#getResolvedFontName--) | 解決されたフォントの名前を取得します。 |
| [setResolvedFontName(String value)](#setResolvedFontName-java.lang.String-) | 解決されたフォントの名前を設定します。 |
### getRequestedFontName() {#getRequestedFontName--}
```
public final String getRequestedFontName()
```


要求されたフォントの名前を取得します。

**Returns:**
java.lang.String - 要求されたフォントの名前。
### getResolvedFontName() {#getResolvedFontName--}
```
public final String getResolvedFontName()
```


解決されたフォントの名前を取得します。ビューのレンダリングに使用されるフォントを制御するために設定できます。

**Returns:**
java.lang.String - フォントが見つかった場合の要求されたフォントの名前、またはフォールバックフォントの名前、フォントが見つからない場合は null。
### setResolvedFontName(String value) {#setResolvedFontName-java.lang.String-}
```
public final void setResolvedFontName(String value)
```


解決されたフォントの名前を設定します。ビューのレンダリングに使用されるフォントを制御するために設定できます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 解決されたフォントの名前。 |

