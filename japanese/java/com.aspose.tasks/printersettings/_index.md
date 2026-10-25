---
title: "PrinterSettings"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "ドキュメントがどのように印刷されるか、印刷するプリンターを含む情報を指定します。"
type: docs
weight: 215
url: /ja/java/com.aspose.tasks/printersettings/
---

**Inheritance:**
java.lang.Object
```
public class PrinterSettings
```

文書がどのように印刷されるかに関する情報を指定します。印刷するプリンターも含まれます。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [PrinterSettings()](#PrinterSettings--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getCollate()](#getCollate--) | 印刷されたドキュメントが段組みかどうかを示す値を取得します。 |
| [getCopies()](#getCopies--) | 印刷するドキュメントの部数を取得します。 |
| [getFromPage()](#getFromPage--) | 印刷する最初のページのページ番号を取得します。 |
| [getPrintFileName()](#getPrintFileName--) | ファイルに印刷する際のファイル名を取得します。 |
| [getPrinterName()](#getPrinterName--) | 使用するプリンターの名前を取得します。 |
| [getSupportsColor()](#getSupportsColor--) | このプリンターがカラー印刷をサポートしているかどうかを示す値を取得します。 |
| [getToPage()](#getToPage--) | 印刷する最後のページ番号を取得します。 |
| [isDefaultPrinter()](#isDefaultPrinter--) | ユーザーが明示的に PrinterName を設定した場合を除き、PrinterName プロパティがデフォルトプリンターを指定しているかどうかを示す値を取得します。 |
| [setCollate(boolean value)](#setCollate-boolean-) | 印刷されたドキュメントが段組みされているかどうかを示す値を設定します。 |
| [setCopies(short value)](#setCopies-short-) | 印刷するドキュメントの部数を設定します。 |
| [setFromPage(int value)](#setFromPage-int-) | 印刷する最初のページのページ番号を設定します。 |
| [setPrintFileName(String value)](#setPrintFileName-java.lang.String-) | ファイルに印刷する際のファイル名を設定します。 |
| [setPrinterName(String value)](#setPrinterName-java.lang.String-) | 使用するプリンターの名前を設定します。 |
| [setToPage(int value)](#setToPage-int-) | 印刷する最後のページ番号を設定します。 |
| [toString()](#toString--) | PrinterSettings に関する情報を文字列形式で提供します。 |
### PrinterSettings() {#PrinterSettings--}
```
public PrinterSettings()
```


### getCollate() {#getCollate--}
```
public boolean getCollate()
```


印刷されたドキュメントが段組みかどうかを示す値を取得します。

**Returns:**
boolean - 印刷されたドキュメントが段組みされているかどうかを示す値。
### getCopies() {#getCopies--}
```
public short getCopies()
```


印刷するドキュメントの部数を取得します。

**Returns:**
short - 印刷するドキュメントの部数。
### getFromPage() {#getFromPage--}
```
public int getFromPage()
```


印刷する最初のページのページ番号を取得します。

**Returns:**
int - 印刷する最初のページのページ番号。
### getPrintFileName() {#getPrintFileName--}
```
public String getPrintFileName()
```


ファイルに印刷する際のファイル名を取得します。

**Returns:**
java.lang.String - ファイルに印刷する際のファイル名。
### getPrinterName() {#getPrinterName--}
```
public String getPrinterName()
```


使用するプリンターの名前を取得します。

**Returns:**
java.lang.String - 使用するプリンターの名前。
### getSupportsColor() {#getSupportsColor--}
```
public boolean getSupportsColor()
```


このプリンターがカラー印刷をサポートしているかどうかを示す値を取得します。

**Returns:**
boolean - このプリンターがカラー印刷をサポートしているかどうかを示す値。
### getToPage() {#getToPage--}
```
public int getToPage()
```


印刷する最後のページ番号を取得します。

**Returns:**
int - 印刷する最後のページ番号。
### isDefaultPrinter() {#isDefaultPrinter--}
```
public boolean isDefaultPrinter()
```


ユーザーが明示的に PrinterName を設定した場合を除き、PrinterName プロパティがデフォルトプリンターを指定しているかどうかを示す値を取得します。

**Returns:**
boolean - PrinterName プロパティがデフォルトプリンターを指定しているかどうかを示す値。
### setCollate(boolean value) {#setCollate-boolean-}
```
public void setCollate(boolean value)
```


印刷されたドキュメントが段組みされているかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | 印刷されたドキュメントが段組みされているかどうかを示す値。 |

### setCopies(short value) {#setCopies-short-}
```
public void setCopies(short value)
```


印刷するドキュメントの部数を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | short | 印刷するドキュメントの部数。 |

### setFromPage(int value) {#setFromPage-int-}
```
public void setFromPage(int value)
```


印刷する最初のページのページ番号を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 印刷する最初のページのページ番号。 |

### setPrintFileName(String value) {#setPrintFileName-java.lang.String-}
```
public void setPrintFileName(String value)
```


ファイルに印刷する際のファイル名を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | ファイルに印刷する際のファイル名。 |

### setPrinterName(String value) {#setPrinterName-java.lang.String-}
```
public void setPrinterName(String value)
```


使用するプリンターの名前を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 使用するプリンターの名前。 |

### setToPage(int value) {#setToPage-int-}
```
public void setToPage(int value)
```


印刷する最後のページ番号を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 印刷する最後のページ番号。 |

### toString() {#toString--}
```
public String toString()
```


PrinterSettings に関する情報を文字列形式で提供します。

**Returns:**
java.lang.String - PrinterSettings に関する情報（文字列形式）。
