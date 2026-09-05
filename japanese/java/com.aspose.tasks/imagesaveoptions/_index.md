---
title: "ImageSaveOptions"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "プロジェクトページを画像にレンダリングする際に追加オプションを指定できます。"
type: docs
weight: 134
url: /ja/java/com.aspose.tasks/imagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class ImageSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

プロジェクトページを画像にレンダリングする際に追加オプションを指定できます。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [ImageSaveOptions(int saveFormat)](#ImageSaveOptions-int-) | TIFF、PNG、BMP、または JPEG 形式でレンダリングされた画像を保存するために使用できる、[ImageSaveOptions](../../com.aspose.tasks/imagesaveoptions) クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getFontSettings()](#getFontSettings--) | プロジェクトのビューをレンダリングする際に使用されるフォント設定を指定します。 |
| [getHorizontalResolution()](#getHorizontalResolution--) | 水平解像度（dpi）を取得します。 |
| [getJpegQuality()](#getJpegQuality--) | JPEG の品質を取得します。 |
| [getPageSavingCallback()](#getPageSavingCallback--) | 各レンダリングページの出力ストリームを取得するために使用されるユーザー定義のコールバックを取得します。 |
| [getPages()](#getPages--) | プロジェクトレイアウトを別々のファイルに保存する際に保存するページ番号のリストを取得します。 |
| [getPixelFormat()](#getPixelFormat--) | 画像内の各ピクセルのカラー データ形式を取得します。 |
| [getReduceFooterGap()](#getReduceFooterGap--) | 最後のタスクとフッターの間のギャップを縮小する必要があるかどうかを示す値を取得します。 |
| [getTiffCompression()](#getTiffCompression--) | 生成された画像を TIFF 形式で保存する際に適用する圧縮タイプを取得します。 |
| [getVerticalResolution()](#getVerticalResolution--) | dpi 単位の垂直解像度を取得します。 |
| [setHorizontalResolution(float value)](#setHorizontalResolution-float-) | dpi 単位の水平解像度を設定します。 |
| [setJpegQuality(int value)](#setJpegQuality-int-) | JPEG の品質を設定します。 |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | 各レンダリングページの出力ストリームを取得するために使用されるユーザー定義のコールバックを設定します。 |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | プロジェクト レイアウトを別々のファイルに保存する際に保存するページ番号のリストを設定します。 |
| [setPixelFormat(int value)](#setPixelFormat-int-) | 画像内の各ピクセルのカラーデータ形式を設定します。 |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | 最後のタスクとフッター間のギャップを縮小するかどうかを示す値を設定します。 |
| [setTiffCompression(int value)](#setTiffCompression-int-) | 生成された画像を TIFF 形式で保存する際に適用する圧縮タイプを設定します。 |
| [setVerticalResolution(float value)](#setVerticalResolution-float-) | dpi 単位の垂直解像度を設定します。 |
### ImageSaveOptions(int saveFormat) {#ImageSaveOptions-int-}
```
public ImageSaveOptions(int saveFormat)
```


TIFF、PNG、BMP、または JPEG 形式でレンダリングされた画像を保存するために使用できる、[ImageSaveOptions](../../com.aspose.tasks/imagesaveoptions) クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| saveFormat | int | TIFF、PNG、BMP、または JPEG[SaveFileFormat](../../com.aspose/tasks/savefileformat) にできます。 |

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
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


プロジェクトのビューをレンダリングする際に使用されるフォント設定を指定します。

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getHorizontalResolution() {#getHorizontalResolution--}
```
public final float getHorizontalResolution()
```


水平解像度（dpi）を取得します。

**Returns:**
float - dpi 単位の水平解像度。
### getJpegQuality() {#getJpegQuality--}
```
public final int getJpegQuality()
```


JPEG の品質を取得します。許容される値の範囲は 0〜100 です。

**Returns:**
int - JPEG の品質。
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


プロジェクトレイアウトを別々のファイルに保存する際に保存するページ番号のリストを取得します。

--------------------

このリストが空の場合、すべてのページが保存されます。

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - プロジェクト レイアウトを別々のファイルに保存する際に保存するページ番号のリスト。
### getPixelFormat() {#getPixelFormat--}
```
public final int getPixelFormat()
```


画像内の各ピクセルのカラー データ形式を取得します。

**Returns:**
int - 画像内の各ピクセルのカラーデータ形式。
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


最後のタスクとフッターの間のギャップを縮小する必要があるかどうかを示す値を取得します。

**Returns:**
boolean - 最後のタスクとフッター間のギャップを縮小するかどうかを示す値。
### getTiffCompression() {#getTiffCompression--}
```
public final int getTiffCompression()
```


生成された画像を TIFF 形式で保存する際に適用する圧縮タイプを取得します。

--------------------

TIFF に保存する場合にのみ有効です。デフォルト値は `TiffCompressionLZW`([getTiffCompression()](../../com.aspose.tasks/imagesaveoptions\#getTiffCompression--)/[setTiffCompression(int)](../../com.aspose.tasks/imagesaveoptions\#setTiffCompression-int-)) です。

**Returns:**
int - 生成された画像を TIFF 形式で保存する際に適用する圧縮タイプ。
### getVerticalResolution() {#getVerticalResolution--}
```
public final float getVerticalResolution()
```


dpi 単位の垂直解像度を取得します。

**Returns:**
float - dpi 単位の垂直解像度。
### setHorizontalResolution(float value) {#setHorizontalResolution-float-}
```
public final void setHorizontalResolution(float value)
```


dpi 単位の水平解像度を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | float | dpi 単位の水平解像度。 |

### setJpegQuality(int value) {#setJpegQuality-int-}
```
public final void setJpegQuality(int value)
```


JPEG の品質を設定します。許容される値の範囲は 0〜100 です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | JPEG の品質。 |

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


プロジェクト レイアウトを別々のファイルに保存する際に保存するページ番号のリストを設定します。

--------------------

このリストが空の場合、すべてのページが保存されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.List&lt;java.lang.Integer&gt; | プロジェクト レイアウトを別々のファイルに保存する際に保存するページ番号のリスト。 |

### setPixelFormat(int value) {#setPixelFormat-int-}
```
public final void setPixelFormat(int value)
```


画像内の各ピクセルのカラーデータ形式を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 画像内の各ピクセルのカラーデータ形式。 |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


最後のタスクとフッター間のギャップを縮小するかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | 最後のタスクとフッター間のギャップを縮小すべきかどうかを示す値。 |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public final void setTiffCompression(int value)
```


生成された画像を TIFF 形式で保存する際に適用する圧縮タイプを設定します。

--------------------

TIFF に保存する場合にのみ有効です。デフォルト値は `TiffCompressionLZW`([getTiffCompression()](../../com.aspose.tasks/imagesaveoptions\#getTiffCompression--)/[setTiffCompression(int)](../../com.aspose.tasks/imagesaveoptions\#setTiffCompression-int-)) です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 生成された画像を TIFF 形式で保存する際に適用する圧縮タイプ。 |

### setVerticalResolution(float value) {#setVerticalResolution-float-}
```
public final void setVerticalResolution(float value)
```


dpi 単位の垂直解像度を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | float | dpi 単位の垂直解像度。 |

