---
title: "HtmlSaveOptions"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "プロジェクトページを HTML にレンダリングする際に追加オプションを指定できます。"
type: docs
weight: 132
url: /ja/java/com.aspose.tasks/htmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class HtmlSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

プロジェクトページを HTML にレンダリングする際に追加オプションを指定できます。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [HtmlSaveOptions()](#HtmlSaveOptions--) | 新しい [HtmlSaveOptions](../../com.aspose.tasks/htmlsaveoptions) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getCssSavingCallback()](#getCssSavingCallback--) | CSS を格納するリソースを作成するために呼び出されるコールバックを取得します。 |
| [getCssStylePrefix()](#getCssStylePrefix--) | CSS スタイルのプレフィックスを取得します。 |
| [getExportCss()](#getExportCss--) | CSS のエクスポート方法を取得します。 |
| [getExportFonts()](#getExportFonts--) | フォントのエクスポート方法を取得します。 |
| [getExportImages()](#getExportImages--) | 画像のエクスポート方法を取得します。 |
| [getFontFaceTypes()](#getFontFaceTypes--) | フォントフェイスの種類を取得します。 |
| [getFontSavingCallback()](#getFontSavingCallback--) | フォントを格納するリソースを作成するために呼び出されるコールバックを取得します。 |
| [getFontSettings()](#getFontSettings--) | プロジェクトのビューをレンダリングする際に使用されるフォント設定を指定します。 |
| [getImageSavingCallback()](#getImageSavingCallback--) | フォントを格納するリソースを作成するために呼び出されるコールバックを取得します。 |
| [getIncludeProjectNameInPageHeader()](#getIncludeProjectNameInPageHeader--) | HTML ページヘッダーにプロジェクト名を含めるかどうかを示す値を取得します。 |
| [getIncludeProjectNameInTitle()](#getIncludeProjectNameInTitle--) | HTML タイトルにプロジェクト名を含めるかどうかを示す値を取得します。 |
| [getPageSavingCallback()](#getPageSavingCallback--) | 各レンダリングページの出力ストリームを取得するために使用されるユーザー定義のコールバックを取得します。 |
| [getPages()](#getPages--) | プロジェクトレイアウトをレンダリングする際に保存するページ番号のリストを取得します。 |
| [getReduceFooterGap()](#getReduceFooterGap--) | 最後のタスクとフッターの間のギャップを縮小する必要があるかどうかを示す値を取得します。 |
| [getUseGradientBrush()](#getUseGradientBrush--) | プロジェクトレイアウトをレンダリングする際にグラデーションブラシを使用するかどうかを示す値を取得します。 |
| [setCssSavingCallback(ICssSavingCallback value)](#setCssSavingCallback-com.aspose.tasks.ICssSavingCallback-) | CSS を格納するリソースを作成するために呼び出されるコールバックを設定します。 |
| [setCssStylePrefix(String value)](#setCssStylePrefix-java.lang.String-) | CSS スタイルのプレフィックスを設定します。 |
| [setExportCss(int value)](#setExportCss-int-) | CSS のエクスポート方法を設定します。 |
| [setExportFonts(int value)](#setExportFonts-int-) | フォントのエクスポート方法を設定します。 |
| [setExportImages(int value)](#setExportImages-int-) | 画像のエクスポート方法を設定します。 |
| [setFontFaceTypes(int value)](#setFontFaceTypes-int-) | フォントフェイスの種類を設定します。 |
| [setFontSavingCallback(IFontSavingCallback value)](#setFontSavingCallback-com.aspose.tasks.IFontSavingCallback-) | フォントを保存するリソースを作成するために呼び出されるコールバックを設定します。 |
| [setImageSavingCallback(IImageSavingCallback value)](#setImageSavingCallback-com.aspose.tasks.IImageSavingCallback-) | フォントを保存するリソースを作成するために呼び出されるコールバックを設定します。 |
| [setIncludeProjectNameInPageHeader(boolean value)](#setIncludeProjectNameInPageHeader-boolean-) | HTML ページヘッダーにプロジェクト名を含めるかどうかを示す値を設定します。 |
| [setIncludeProjectNameInTitle(boolean value)](#setIncludeProjectNameInTitle-boolean-) | HTML タイトルにプロジェクト名を含めるかどうかを示す値を設定します。 |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | 各レンダリングページの出力ストリームを取得するために使用されるユーザー定義のコールバックを設定します。 |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | プロジェクトレイアウトをレンダリングする際に保存するページ番号のリストを設定します。 |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | 最後のタスクとフッター間のギャップを縮小するかどうかを示す値を設定します。 |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | プロジェクトレイアウトをレンダリングする際にグラデーションブラシを使用するかどうかを示す値を設定します。 |
### HtmlSaveOptions() {#HtmlSaveOptions--}
```
public HtmlSaveOptions()
```


新しい [HtmlSaveOptions](../../com.aspose.tasks/htmlsaveoptions) クラスのインスタンスを初期化します。

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
public SaveOptions deepClone()
```


内部使用のために予約されています。

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getCssSavingCallback() {#getCssSavingCallback--}
```
public final ICssSavingCallback getCssSavingCallback()
```


CSS を格納するリソースを作成するために呼び出されるコールバックを取得します。

**Returns:**
[ICssSavingCallback](../../com.aspose.tasks/icsssavingcallback) - the callback that is called to create resource to store CSS.
### getCssStylePrefix() {#getCssStylePrefix--}
```
public final String getCssStylePrefix()
```


CSS スタイルのプレフィックスを取得します。

**Returns:**
java.lang.String - CSS スタイルプレフィックス。
### getExportCss() {#getExportCss--}
```
public final int getExportCss()
```


CSS のエクスポート方法を取得します。

**Returns:**
int - CSS のエクスポート方法。
### getExportFonts() {#getExportFonts--}
```
public final int getExportFonts()
```


フォントのエクスポート方法を取得します。

**Returns:**
int - フォントのエクスポート方法。
### getExportImages() {#getExportImages--}
```
public final int getExportImages()
```


画像のエクスポート方法を取得します。

**Returns:**
int - 画像のエクスポート方法。
### getFontFaceTypes() {#getFontFaceTypes--}
```
public final int getFontFaceTypes()
```


フォントフェイスの種類を取得します。

値: フォントフェイスの種類。

**Returns:**
int - フォントフェイスの種類。
### getFontSavingCallback() {#getFontSavingCallback--}
```
public final IFontSavingCallback getFontSavingCallback()
```


フォントを格納するリソースを作成するために呼び出されるコールバックを取得します。

**Returns:**
[IFontSavingCallback](../../com.aspose.tasks/ifontsavingcallback) - the callback that is called to create resource to store font.
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


プロジェクトのビューをレンダリングする際に使用されるフォント設定を指定します。

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getImageSavingCallback() {#getImageSavingCallback--}
```
public final IImageSavingCallback getImageSavingCallback()
```


フォントを格納するリソースを作成するために呼び出されるコールバックを取得します。

**Returns:**
[IImageSavingCallback](../../com.aspose.tasks/iimagesavingcallback) - the callback that is called to create resource to store font.
### getIncludeProjectNameInPageHeader() {#getIncludeProjectNameInPageHeader--}
```
public final boolean getIncludeProjectNameInPageHeader()
```


HTML ページヘッダーにプロジェクト名を含めるかどうかを示す値を取得します。

**Returns:**
boolean - HTML ページヘッダーにプロジェクト名を含めるかどうかを示す値。
### getIncludeProjectNameInTitle() {#getIncludeProjectNameInTitle--}
```
public final boolean getIncludeProjectNameInTitle()
```


HTML タイトルにプロジェクト名を含めるかどうかを示す値を取得します。

**Returns:**
boolean - HTML タイトルにプロジェクト名を含めるかどうかを示す値。
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


各レンダリングページの出力ストリームを取得するために使用されるユーザー定義のコールバックを取得します。

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined callback which is used to get an output stream for each rendered page.
### getPages() {#getPages--}
```
public final List<Integer> getPages()
```


プロジェクトレイアウトをレンダリングする際に保存するページ番号のリストを取得します。

--------------------

このリストが空の場合、すべてのプロジェクトページが保存されます。

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - プロジェクトレイアウトをレンダリングする際に保存するページ番号のリスト。
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


最後のタスクとフッターの間のギャップを縮小する必要があるかどうかを示す値を取得します。

**Returns:**
boolean - 最後のタスクとフッター間のギャップを縮小するかどうかを示す値。
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


プロジェクトレイアウトをレンダリングする際にグラデーションブラシを使用するかどうかを示す値を取得します。

--------------------

現在、HTML へのレンダリング時にグラデーションブラシの使用はサポートされていません。

**Returns:**
boolean - プロジェクトレイアウトをレンダリングする際にグラデーションブラシを使用するかどうかを示す値。
### setCssSavingCallback(ICssSavingCallback value) {#setCssSavingCallback-com.aspose.tasks.ICssSavingCallback-}
```
public final void setCssSavingCallback(ICssSavingCallback value)
```


CSS を格納するリソースを作成するために呼び出されるコールバックを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [ICssSavingCallback](../../com.aspose.tasks/icsssavingcallback) | CSS を保存するリソースを作成するために呼び出されるコールバック。 |

### setCssStylePrefix(String value) {#setCssStylePrefix-java.lang.String-}
```
public final void setCssStylePrefix(String value)
```


CSS スタイルのプレフィックスを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | CSS スタイルプレフィックス。 |

### setExportCss(int value) {#setExportCss-int-}
```
public final void setExportCss(int value)
```


CSS のエクスポート方法を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | CSS のエクスポート方法。 |

### setExportFonts(int value) {#setExportFonts-int-}
```
public final void setExportFonts(int value)
```


フォントのエクスポート方法を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | フォントのエクスポート方法。 |

### setExportImages(int value) {#setExportImages-int-}
```
public final void setExportImages(int value)
```


画像のエクスポート方法を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 画像のエクスポート方法。 |

### setFontFaceTypes(int value) {#setFontFaceTypes-int-}
```
public final void setFontFaceTypes(int value)
```


フォントフェイスの種類を設定します。

値: フォントフェイスの種類。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | フォントフェイスの種類。 |

### setFontSavingCallback(IFontSavingCallback value) {#setFontSavingCallback-com.aspose.tasks.IFontSavingCallback-}
```
public final void setFontSavingCallback(IFontSavingCallback value)
```


フォントを保存するリソースを作成するために呼び出されるコールバックを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [IFontSavingCallback](../../com.aspose.tasks/ifontsavingcallback) | フォントを保存するリソースを作成するために呼び出されるコールバック。 |

### setImageSavingCallback(IImageSavingCallback value) {#setImageSavingCallback-com.aspose.tasks.IImageSavingCallback-}
```
public final void setImageSavingCallback(IImageSavingCallback value)
```


フォントを保存するリソースを作成するために呼び出されるコールバックを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [IImageSavingCallback](../../com.aspose.tasks/iimagesavingcallback) | フォントを保存するリソースを作成するために呼び出されるコールバック。 |

### setIncludeProjectNameInPageHeader(boolean value) {#setIncludeProjectNameInPageHeader-boolean-}
```
public final void setIncludeProjectNameInPageHeader(boolean value)
```


HTML ページヘッダーにプロジェクト名を含めるかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | HTML ページヘッダーにプロジェクト名を含めるかどうかを示す値。 |

### setIncludeProjectNameInTitle(boolean value) {#setIncludeProjectNameInTitle-boolean-}
```
public final void setIncludeProjectNameInTitle(boolean value)
```


HTML タイトルにプロジェクト名を含めるかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | HTML タイトルにプロジェクト名を含めるかどうかを示す値。 |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


各レンダリングページの出力ストリームを取得するために使用されるユーザー定義のコールバックを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | 各レンダリングページの出力ストリームを取得するために使用されるユーザー定義コールバック。 |

### setPages(List&lt;Integer&gt; value) {#setPages-java.util.List-java.lang.Integer--}
```
public final void setPages(List<Integer> value)
```


プロジェクトレイアウトをレンダリングする際に保存するページ番号のリストを設定します。

--------------------

このリストが空の場合、すべてのプロジェクトページが保存されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.List&lt;java.lang.Integer&gt; | プロジェクトレイアウトをレンダリングする際に保存するページ番号のリスト。 |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


最後のタスクとフッター間のギャップを縮小するかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | 最後のタスクとフッター間のギャップを縮小すべきかどうかを示す値。 |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


プロジェクトレイアウトをレンダリングする際にグラデーションブラシを使用するかどうかを示す値を設定します。

--------------------

現在、HTML へのレンダリング時にグラデーションブラシの使用はサポートされていません。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | プロジェクトレイアウトをレンダリングする際にグラデーションブラシを使用するかどうかを示す値。 |

