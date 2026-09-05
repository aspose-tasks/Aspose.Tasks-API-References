---
title: "PdfSaveOptions"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "プロジェクトページを PDF にレンダリングする際に追加オプションを指定できます。"
type: docs
weight: 191
url: /ja/java/com.aspose.tasks/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class PdfSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

プロジェクトページを PDF にレンダリングする際に追加オプションを指定できます。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | ドキュメントを [SaveFileFormat](../../com.aspose.tasks/savefileformat) 形式で保存するために使用できる [PdfSaveOptions](../../com.aspose.tasks/pdfsaveoptions) クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getCompliance()](#getCompliance--) | 生成された PDF ドキュメントの目的のコンプライアンス レベルを取得します。 |
| [getEncryptionDetails()](#getEncryptionDetails--) | 暗号化の詳細を取得します。 |
| [getFontSettings()](#getFontSettings--) | プロジェクトのビューをレンダリングする際に使用されるフォント設定を指定します。 |
| [getPageSavingCallback()](#getPageSavingCallback--) | 各レンダリングページの出力ストリームを取得するために使用されるユーザー定義のコールバックを取得します。 |
| [getPages()](#getPages--) | プロジェクト レイアウトを別々のファイルに保存する際に保存するページ番号のリストを取得します。 |
| [getReduceFooterGap()](#getReduceFooterGap--) | 最後のタスクとフッターの間のギャップを縮小する必要があるかどうかを示す値を取得します。 |
| [getSaveToSeparateFiles()](#getSaveToSeparateFiles--) | プロジェクト ページを別々のファイルに保存するかどうかを示す値を取得します。 |
| [getTextCompression()](#getTextCompression--) | 画像を除くすべてのコンテンツ ストリームで使用される圧縮タイプを取得します。 |
| [setCompliance(int value)](#setCompliance-int-) | 生成された PDF ドキュメントの目的のコンプライアンス レベルを設定します。 |
| [setEncryptionDetails(PdfEncryptionDetails value)](#setEncryptionDetails-com.aspose.tasks.PdfEncryptionDetails-) | 暗号化の詳細を設定します。 |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | 各レンダリングページの出力ストリームを取得するために使用されるユーザー定義のコールバックを設定します。 |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | プロジェクト レイアウトを別々のファイルに保存する際に保存するページ番号のリストを設定します。 |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | 最後のタスクとフッター間のギャップを縮小するかどうかを示す値を設定します。 |
| [setSaveToSeparateFiles(boolean value)](#setSaveToSeparateFiles-boolean-) | プロジェクト ページを別々のファイルに保存するかどうかを示す値を設定します。 |
| [setTextCompression(int value)](#setTextCompression-int-) | 画像を除くすべてのコンテンツ ストリームで使用される圧縮タイプを設定します。 |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


ドキュメントを [SaveFileFormat](../../com.aspose.tasks/savefileformat) 形式で保存するために使用できる [PdfSaveOptions](../../com.aspose.tasks/pdfsaveoptions) クラスの新しいインスタンスを初期化します。

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public void copyOutputPropertiesFrom(SaveOptions source)
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
### getCompliance() {#getCompliance--}
```
public final int getCompliance()
```


生成された PDF ドキュメントの目的のコンプライアンス レベルを取得します。デフォルトは [PdfCompliance.Pdf15](../../com.aspose.tasks/pdfcompliance\#Pdf15) です。

**Returns:**
int - 生成された PDF ドキュメントの目的のコンプライアンス レベル。
### getEncryptionDetails() {#getEncryptionDetails--}
```
public final PdfEncryptionDetails getEncryptionDetails()
```


暗号化の詳細を取得します。設定されていない場合、暗号化は実行されません。

**Returns:**
[PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) - an encryption details.
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


プロジェクトのビューをレンダリングする際に使用されるフォント設定を指定します。

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


各レンダリングページの出力ストリームを取得するために使用されるユーザー定義コールバックを取得します。`SaveToSeparateFiles`([getSaveToSeparateFiles()](../../com.aspose.tasks/pdfsaveoptions\#getSaveToSeparateFiles--)/[setSaveToSeparateFiles(boolean)](../../com.aspose.tasks/pdfsaveoptions\#setSaveToSeparateFiles-boolean-)) オプションが使用されている場合に適用されます。

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined callback which is used to get an output stream for each rendered page.
### getPages() {#getPages--}
```
public final List<Integer> getPages()
```


プロジェクト レイアウトを別々のファイルに保存する際に保存するページ番号のリストを取得します。

--------------------

このリストが空の場合、すべてのページが保存されます。

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - プロジェクト レイアウトを別々のファイルに保存する際に保存するページ番号のリスト。
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


最後のタスクとフッターの間のギャップを縮小する必要があるかどうかを示す値を取得します。

**Returns:**
boolean - 最後のタスクとフッター間のギャップを縮小するかどうかを示す値。
### getSaveToSeparateFiles() {#getSaveToSeparateFiles--}
```
public final boolean getSaveToSeparateFiles()
```


プロジェクト ページを別々のファイルに保存するかどうかを示す値を取得します。

**Returns:**
boolean - プロジェクト ページを別々のファイルに保存するかどうかを示す値。
### getTextCompression() {#getTextCompression--}
```
public final int getTextCompression()
```


画像を除くすべてのコンテンツ ストリームで使用される圧縮タイプを取得します。デフォルトは [PdfTextCompression.Flate](../../com.aspose.tasks/pdftextcompression\#Flate) です。

**Returns:**
int - 画像を除くすべてのコンテンツ ストリームで使用される圧縮タイプ。
### setCompliance(int value) {#setCompliance-int-}
```
public final void setCompliance(int value)
```


生成された PDF ドキュメントの目的のコンプライアンス レベルを設定します。デフォルトは [PdfCompliance.Pdf15](../../com.aspose.tasks/pdfcompliance\#Pdf15) です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 生成された PDF ドキュメントの目的のコンプライアンス レベル。 |

### setEncryptionDetails(PdfEncryptionDetails value) {#setEncryptionDetails-com.aspose.tasks.PdfEncryptionDetails-}
```
public final void setEncryptionDetails(PdfEncryptionDetails value)
```


暗号化の詳細を設定します。設定されていない場合、暗号化は実行されません。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) | 暗号化の詳細。 |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


各レンダリングページの出力ストリームを取得するために使用されるユーザー定義コールバックを設定します。`SaveToSeparateFiles`([getSaveToSeparateFiles()](../../com.aspose.tasks/pdfsaveoptions\#getSaveToSeparateFiles--)/[setSaveToSeparateFiles(boolean)](../../com.aspose.tasks/pdfsaveoptions\#setSaveToSeparateFiles-boolean-)) オプションが使用されている場合に適用されます。

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

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


最後のタスクとフッター間のギャップを縮小するかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | 最後のタスクとフッター間のギャップを縮小すべきかどうかを示す値。 |

### setSaveToSeparateFiles(boolean value) {#setSaveToSeparateFiles-boolean-}
```
public final void setSaveToSeparateFiles(boolean value)
```


プロジェクト ページを別々のファイルに保存するかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | プロジェクトページを別々のファイルに保存するかどうかを示す値。 |

### setTextCompression(int value) {#setTextCompression-int-}
```
public final void setTextCompression(int value)
```


画像を除くすべてのコンテンツストリームに使用される圧縮タイプを設定します。デフォルトは [PdfTextCompression.Flate](../../com.aspose.tasks/pdftextcompression\\#Flate) です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 画像を除くすべてのコンテンツストリームに使用される圧縮タイプ。 |

