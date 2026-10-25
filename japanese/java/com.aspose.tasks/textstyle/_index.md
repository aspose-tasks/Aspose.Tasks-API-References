---
title: "TextStyle"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "プロジェクトビュー内の項目のテキストの視覚スタイルを変更します。"
type: docs
weight: 315
url: /ja/java/com.aspose.tasks/textstyle/
---

**Inheritance:**
java.lang.Object
```
public class TextStyle
```

プロジェクトビュー内の項目のテキストの視覚スタイルを変更します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [TextStyle()](#TextStyle--) | デフォルト設定で [TextStyle](../../com.aspose/tasks/textstyle) クラスの新しいインスタンスを初期化します。 |
| [TextStyle(float fontSize, int fontStyle)](#TextStyle-float-int-) | デフォルトフォントと指定されたフォントサイズおよびスタイルで [TextStyle](../../com.aspose/tasks/textstyle) クラスの新しいインスタンスを初期化します。 |
| [TextStyle(int fontStyle)](#TextStyle-int-) | デフォルトフォントと指定されたフォントスタイルで [TextStyle](../../com.aspose/tasks/textstyle) クラスの新しいインスタンスを初期化します。 |
| [TextStyle(FontDescriptor font)](#TextStyle-com.aspose.tasks.FontDescriptor-) | 指定されたフォント設定で [TextStyle](../../com.aspose/tasks/textstyle) クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getBackgroundColor()](#getBackgroundColor--) | テキストスタイルの背景色を取得します。 |
| [getBackgroundPattern()](#getBackgroundPattern--) | テキストスタイルの背景パターンを取得します。 |
| [getColor()](#getColor--) | テキストの色を取得します。 |
| [getFont()](#getFont--) | テキストスタイルのフォントを取得します。 |
| [getItemType()](#getItemType--) | テキストスタイルの [TextItemType](../../com.aspose/tasks/textitemtype) を取得します。 |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | テキストスタイルの背景色を設定します。 |
| [setBackgroundPattern(int value)](#setBackgroundPattern-int-) | テキストスタイルの背景パターンを設定します。 |
| [setColor(Color value)](#setColor-java.awt.Color-) | テキストの色を設定します。 |
| [setFont(FontDescriptor value)](#setFont-com.aspose.tasks.FontDescriptor-) | テキストスタイルのフォントを設定します。 |
| [setItemType(int value)](#setItemType-int-) | テキストスタイルの [TextItemType](../../com.aspose/tasks/textitemtype) を設定します。 |
### TextStyle() {#TextStyle--}
```
public TextStyle()
```


デフォルト設定で [TextStyle](../../com.aspose/tasks/textstyle) クラスの新しいインスタンスを初期化します。

### TextStyle(float fontSize, int fontStyle) {#TextStyle-float-int-}
```
public TextStyle(float fontSize, int fontStyle)
```


デフォルトフォントと指定されたフォントサイズおよびスタイルで [TextStyle](../../com.aspose/tasks/textstyle) クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fontSize | float | TextStyle のフォントサイズ。 |
| fontStyle | int | TextStyle のフォントスタイル。 |

### TextStyle(int fontStyle) {#TextStyle-int-}
```
public TextStyle(int fontStyle)
```


デフォルトフォントと指定されたフォントスタイルで [TextStyle](../../com.aspose/tasks/textstyle) クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fontStyle | int | デフォルトフォントに適用するフォントスタイル。 |

### TextStyle(FontDescriptor font) {#TextStyle-com.aspose.tasks.FontDescriptor-}
```
public TextStyle(FontDescriptor font)
```


指定されたフォント設定で [TextStyle](../../com.aspose/tasks/textstyle) クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| font | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | TextStyle のフォント。 |

### getBackgroundColor() {#getBackgroundColor--}
```
public final Color getBackgroundColor()
```


テキストスタイルの背景色を取得します。 `Color`([getBackgroundColor()](../../com.aspose/tasks/textstyle\#getBackgroundColor--)/[setBackgroundColor(java.awt.Color)](../../com.aspose/tasks/textstyle\#setBackgroundColor-java.awt.Color-)).

**Returns:**
java.awt.Color - テキストスタイルの背景色。
### getBackgroundPattern() {#getBackgroundPattern--}
```
public final int getBackgroundPattern()
```


テキストスタイルの背景パターンを取得します。 `BackgroundPattern`([getBackgroundPattern()](../../com.aspose/tasks/textstyle\#getBackgroundPattern--)/[setBackgroundPattern(int)](../../com.aspose/tasks/textstyle\#setBackgroundPattern-int-)).

**Returns:**
int - テキストスタイルの背景パターン。
### getColor() {#getColor--}
```
public final Color getColor()
```


テキストの色を取得します。

**Returns:**
java.awt.Color - テキストの色。
### getFont() {#getFont--}
```
public final FontDescriptor getFont()
```


テキストスタイルのフォントを取得します。

**Returns:**
[FontDescriptor](../../com.aspose.tasks/fontdescriptor) - font of the text style.
### getItemType() {#getItemType--}
```
public int getItemType()
```


テキストスタイルの [TextItemType](../../com.aspose/tasks/textitemtype) を取得します。

**Returns:**
int - テキストスタイルの[TextItemType](../../com.aspose/tasks/textitemtype)。
### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public final void setBackgroundColor(Color value)
```


テキストスタイルの背景色を設定します。 `Color`([getBackgroundColor()](../../com.aspose.tasks/textstyle\\#getBackgroundColor--)/[setBackgroundColor(java.awt.Color)](../../com.aspose.tasks/textstyle\\#setBackgroundColor-java.awt.Color-)).

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.awt.Color | テキストスタイルの背景色。 |

### setBackgroundPattern(int value) {#setBackgroundPattern-int-}
```
public final void setBackgroundPattern(int value)
```


テキストスタイルの背景パターンを設定します。 `BackgroundPattern`([getBackgroundPattern()](../../com.aspose.tasks/textstyle\\#getBackgroundPattern--)/[setBackgroundPattern(int)](../../com.aspose.tasks/textstyle\\#setBackgroundPattern-int-)).

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | テキストスタイルの背景パターン。 |

### setColor(Color value) {#setColor-java.awt.Color-}
```
public final void setColor(Color value)
```


テキストの色を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.awt.Color | テキストの色。 |

### setFont(FontDescriptor value) {#setFont-com.aspose.tasks.FontDescriptor-}
```
public final void setFont(FontDescriptor value)
```


テキストスタイルのフォントを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | テキストスタイルのフォント。 |

### setItemType(int value) {#setItemType-int-}
```
public void setItemType(int value)
```


テキストスタイルの [TextItemType](../../com.aspose/tasks/textitemtype) を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | int | テキストスタイルの[TextItemType](../../com.aspose.tasks/textitemtype)。 |

