---
title: "SvgOptions"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "プロジェクトページを SVG にレンダリングする際に追加オプションを指定できます。"
type: docs
weight: 283
url: /ja/java/com.aspose.tasks/svgoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.ICloneableSaveOptions
```
public class SvgOptions extends SaveOptions implements ICloneableSaveOptions
```

プロジェクトページを SVG にレンダリングする際に追加オプションを指定できます。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [SvgOptions()](#SvgOptions--) | SVG形式でプロジェクトを保存できる [SvgOptions](../../com.aspose.tasks/svgoptions) クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getPageSavingCallback()](#getPageSavingCallback--) | 各レンダリングページの出力ストリームを取得するために使用される、ユーザー定義の実装コールバックを取得します。 |
| [getUseGradientBrush()](#getUseGradientBrush--) | プロジェクトレイアウトのレンダリング時にグラデーションブラシを使用するかどうかを決定します。 |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | 各レンダリングページの出力ストリームを取得するために使用される、ユーザー定義の実装コールバックを設定します。 |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | プロジェクトレイアウトのレンダリング時にグラデーションブラシを使用するかどうかを決定します。 |
### SvgOptions() {#SvgOptions--}
```
public SvgOptions()
```


SVG形式でプロジェクトを保存できる [SvgOptions](../../com.aspose.tasks/svgoptions) クラスの新しいインスタンスを初期化します。

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
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


各レンダリングページの出力ストリームを取得するために使用される、ユーザー定義の実装コールバックを取得します。

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined implementation callback which is used to get an output stream for each rendered page.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


プロジェクトレイアウトのレンダリング時にグラデーションブラシを使用するかどうかを決定します。

--------------------

現在、SVGへのレンダリングでグラデーションブラシの使用はサポートされていません。

**Returns:**
boolean - プロジェクトレイアウトのレンダリング時にグラデーションブラシを使用するかどうかを示す値。
### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


各レンダリングページの出力ストリームを取得するために使用される、ユーザー定義の実装コールバックを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | 各レンダリングページの出力ストリームを取得するために使用される、ユーザー定義の実装コールバック。 |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


プロジェクトレイアウトのレンダリング時にグラデーションブラシを使用するかどうかを決定します。

--------------------

現在、SVGへのレンダリングでグラデーションブラシの使用はサポートされていません。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | プロジェクトレイアウトのレンダリング時にグラデーションブラシを使用するかどうかを示す値。 |

