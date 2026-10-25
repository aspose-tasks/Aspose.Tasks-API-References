---
title: "PageSettings"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "プロジェクトビューのページの印刷設定を表します。"
type: docs
weight: 181
url: /ja/java/com.aspose.tasks/pagesettings/
---

**Inheritance:**
java.lang.Object
```
public class PageSettings
```

プロジェクトビューのページの印刷設定を表します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [PageSettings()](#PageSettings--) | 新しい [PageSettings](../../com.aspose.tasks/pagesettings) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getAdjustToPercentOfNormalSize()](#getAdjustToPercentOfNormalSize--) | 印刷を指定されたパーセンテージ（`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) の通常サイズに調整するかどうかを示す値を取得します。 |
| [getFirstPageNumber()](#getFirstPageNumber--) | 印刷の最初のページ番号を取得します。 |
| [getPagesInHeight()](#getPagesInHeight--) | 印刷する高さ方向のページ数を取得します。 |
| [getPagesInWidth()](#getPagesInWidth--) | 印刷する幅方向のページ数を取得します。 |
| [getPaperSize()](#getPaperSize--) | 用紙サイズを取得します。 |
| [getPaperSizeId()](#getPaperSizeId--) | PrinterPaperSize のいずれかの値またはカスタムページサイズ ID を表す整数を取得します。 |
| [getPercentOfNormalSize()](#getPercentOfNormalSize--) | 印刷を調整する通常サイズのパーセンテージを取得します。 |
| [isPortrait()](#isPortrait--) | ページの向きが縦向きかどうかを示す値を取得します。ページの向きが横向きの場合は false を返します。 |
| [setAdjustToPercentOfNormalSize(boolean value)](#setAdjustToPercentOfNormalSize-boolean-) | 印刷を指定されたパーセンテージ（`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) の通常サイズに調整するかどうかを示す値を設定します。 |
| [setFirstPageNumber(short value)](#setFirstPageNumber-short-) | 印刷の最初のページ番号を設定します。 |
| [setPagesInHeight(int value)](#setPagesInHeight-int-) | 印刷する高さ方向のページ数を設定します。 |
| [setPagesInWidth(int value)](#setPagesInWidth-int-) | 印刷する幅方向のページ数を設定します。 |
| [setPaperSize(int value)](#setPaperSize-int-) | 用紙サイズを設定します。 |
| [setPaperSizeId(int value)](#setPaperSizeId-int-) | PrinterPaperSize のいずれかの値またはカスタムページサイズ ID を表す整数を設定します。 |
| [setPercentOfNormalSize(int value)](#setPercentOfNormalSize-int-) | 印刷を調整する通常サイズのパーセンテージを設定します。 |
| [setPortrait(boolean value)](#setPortrait-boolean-) | ページの向きが縦向きかどうかを示す値を設定します。ページの向きが横向きの場合は false を返します。 |
### PageSettings() {#PageSettings--}
```
public PageSettings()
```


新しい [PageSettings](../../com.aspose/tasks/pagesettings) クラスのインスタンスを初期化します。プロジェクトビューのページの印刷設定を表します。

### getAdjustToPercentOfNormalSize() {#getAdjustToPercentOfNormalSize--}
```
public final boolean getAdjustToPercentOfNormalSize()
```


印刷を指定されたパーセンテージ（`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) の通常サイズに調整するかどうかを示す値を取得します。

--------------------

プロジェクトが HTML 形式でレンダリングされる場合は効果がありません。

**Returns:**
boolean - 指定されたパーセンテージ（`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) の通常サイズに印刷を調整するかどうかを示す値です。
### getFirstPageNumber() {#getFirstPageNumber--}
```
public final short getFirstPageNumber()
```


印刷の最初のページ番号を取得します。

**Returns:**
short - 印刷の最初のページ番号です。
### getPagesInHeight() {#getPagesInHeight--}
```
public final int getPagesInHeight()
```


印刷する高さ方向のページ数を取得します。

**Returns:**
int - 印刷する高さ方向のページ数です。
### getPagesInWidth() {#getPagesInWidth--}
```
public final int getPagesInWidth()
```


印刷する幅方向のページ数を取得します。

**Returns:**
int - 印刷する幅方向のページ数です。
### getPaperSize() {#getPaperSize--}
```
public final int getPaperSize()
```


用紙サイズを取得します。[PrinterPaperSize](../../com.aspose/tasks/printerpapersize) 列挙体のいずれかの値になる可能性があります。

**Returns:**
int - 用紙サイズです。
### getPaperSizeId() {#getPaperSizeId--}
```
public final int getPaperSizeId()
```


PrinterPaperSize のいずれかの値またはカスタムページサイズ ID を表す整数を取得します。この値は OS 設定から PaperSize を取得するために使用できます。

**Returns:**
int - PrinterPaperSize のいずれかの値またはカスタムページサイズ ID を表す整数です。
### getPercentOfNormalSize() {#getPercentOfNormalSize--}
```
public final int getPercentOfNormalSize()
```


印刷を調整する通常サイズのパーセンテージを取得します。

**Returns:**
int - 印刷を調整する標準サイズのパーセンテージです。
### isPortrait() {#isPortrait--}
```
public final boolean isPortrait()
```


ページの向きが縦向きかどうかを示す値を取得します。ページの向きが横向きの場合は false を返します。

--------------------

SaveOptions.getPageSize() == PageSize.DefinedInView の場合、レンダリング中に適用されます。

**Returns:**
boolean - ページの向きが縦向きかどうかを示す値です。横向きの場合は false を返します。
### setAdjustToPercentOfNormalSize(boolean value) {#setAdjustToPercentOfNormalSize-boolean-}
```
public final void setAdjustToPercentOfNormalSize(boolean value)
```


印刷を指定されたパーセンテージ（`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) の通常サイズに調整するかどうかを示す値を設定します。

--------------------

プロジェクトが HTML 形式でレンダリングされる場合は効果がありません。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | boolean | 指定されたパーセンテージ（`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose.tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose.tasks/pagesettings\#setPercentOfNormalSize-int-))）の標準サイズに印刷を調整するかどうかを示す値です。 |

### setFirstPageNumber(short value) {#setFirstPageNumber-short-}
```
public final void setFirstPageNumber(short value)
```


印刷の最初のページ番号を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | short | 印刷の開始ページ番号です。 |

### setPagesInHeight(int value) {#setPagesInHeight-int-}
```
public final void setPagesInHeight(int value)
```


印刷する高さ方向のページ数を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 印刷する高さ方向のページ数です。 |

### setPagesInWidth(int value) {#setPagesInWidth-int-}
```
public final void setPagesInWidth(int value)
```


印刷する幅方向のページ数を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 印刷する幅方向のページ数です。 |

### setPaperSize(int value) {#setPaperSize-int-}
```
public final void setPaperSize(int value)
```


用紙サイズを設定します。[PrinterPaperSize](../../com.aspose.tasks/printerpapersize) 列挙体のいずれかの値にすることができます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 用紙サイズです。 |

### setPaperSizeId(int value) {#setPaperSizeId-int-}
```
public final void setPaperSizeId(int value)
```


PrinterPaperSize のいずれかの値またはカスタムページサイズ ID を表す整数を設定します。この値は OS 設定から PaperSize を取得するために使用できます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | PrinterPaperSize のいずれかの値またはカスタムページサイズ ID を表す整数です。 |

### setPercentOfNormalSize(int value) {#setPercentOfNormalSize-int-}
```
public final void setPercentOfNormalSize(int value)
```


印刷を調整する通常サイズのパーセンテージを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 印刷を調整する標準サイズのパーセンテージです。 |

### setPortrait(boolean value) {#setPortrait-boolean-}
```
public final void setPortrait(boolean value)
```


ページの向きが縦向きかどうかを示す値を設定します。ページの向きが横向きの場合は false を返します。

--------------------

SaveOptions.getPageSize() == PageSize.DefinedInView の場合、レンダリング中に適用されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | ページの向きが縦向きかどうかを示す値です。横向きの場合は false を返します。 |

