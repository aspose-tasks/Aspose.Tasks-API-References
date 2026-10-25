---
title: "PageInfo"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "MPP ファイル形式に存在し、印刷に使用されるページ設定データを表します。"
type: docs
weight: 176
url: /ja/java/com.aspose.tasks/pageinfo/
---

**Inheritance:**
java.lang.Object
```
public class PageInfo
```

MPP ファイル形式に存在し、印刷に使用されるページ設定データを表します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [PageInfo()](#PageInfo--) | 新しい [PageInfo](../../com.aspose.tasks/pageinfo) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getFooter()](#getFooter--) | フッターデータを表す [HeaderFooterInfo](../../com.aspose/tasks/headerfooterinfo) クラスのインスタンスを取得します。 |
| [getHeader()](#getHeader--) | ヘッダーデータを表す [HeaderFooterInfo](../../com.aspose/tasks/headerfooterinfo) クラスのインスタンスを取得します。 |
| [getLegend()](#getLegend--) | ページ凡例の描画オプションを指定する [PageLegend](../../com.aspose/tasks/pagelegend) クラスのインスタンスを取得します。 |
| [getMargins()](#getMargins--) | ページ余白を指定する [PageMargins](../../com.aspose/tasks/pagemargins) クラスのインスタンスを取得します。 |
| [getName()](#getName--) | 設定データが使用されるビューの名前を取得します。 |
| [getPageSettings()](#getPageSettings--) | `PageSettings`([getPageSettings()](../../com.aspose/tasks/pageinfo\#getPageSettings--)) クラスのインスタンスを取得します。このクラスはページ印刷設定を指定します。 |
| [getPageViewSettings()](#getPageViewSettings--) | `PageViewSettings`([getPageViewSettings()](../../com.aspose/tasks/pageinfo\#getPageViewSettings--)) クラスのインスタンスを取得します。このクラスはページビュー印刷設定を指定します。 |
| [setFooter(HeaderFooterInfo value)](#setFooter-com.aspose.tasks.HeaderFooterInfo-) | フッターデータを表す [HeaderFooterInfo](../../com.aspose/tasks/headerfooterinfo) クラスのインスタンスを設定します。 |
| [setHeader(HeaderFooterInfo value)](#setHeader-com.aspose.tasks.HeaderFooterInfo-) | ヘッダーデータを表す [HeaderFooterInfo](../../com.aspose/tasks/headerfooterinfo) クラスのインスタンスを設定します。 |
| [setLegend(PageLegend value)](#setLegend-com.aspose.tasks.PageLegend-) | ページ凡例の描画オプションを指定する [PageLegend](../../com.aspose/tasks/pagelegend) クラスのインスタンスを設定します。 |
### PageInfo() {#PageInfo--}
```
public PageInfo()
```


[PageInfo](../../com.aspose/tasks/pageinfo) クラスの新しいインスタンスを初期化します。このクラスは MPP ファイル形式に存在し、印刷に使用されるページ設定データを表します。

### getFooter() {#getFooter--}
```
public final HeaderFooterInfo getFooter()
```


フッターデータを表す [HeaderFooterInfo](../../com.aspose/tasks/headerfooterinfo) クラスのインスタンスを取得します。

**Returns:**
[HeaderFooterInfo](../../com.aspose.tasks/headerfooterinfo) - an instance of the [HeaderFooterInfo](../../com.aspose.tasks/headerfooterinfo) class which represents a footer data.
### getHeader() {#getHeader--}
```
public final HeaderFooterInfo getHeader()
```


ヘッダーデータを表す [HeaderFooterInfo](../../com.aspose/tasks/headerfooterinfo) クラスのインスタンスを取得します。

**Returns:**
[HeaderFooterInfo](../../com.aspose.tasks/headerfooterinfo) - the instance of the [HeaderFooterInfo](../../com.aspose.tasks/headerfooterinfo) class which represents a header data.
### getLegend() {#getLegend--}
```
public final PageLegend getLegend()
```


ページ凡例の描画オプションを指定する [PageLegend](../../com.aspose/tasks/pagelegend) クラスのインスタンスを取得します。

--------------------

現在、ガントチャートビューにのみ適用されます。

**Returns:**
[PageLegend](../../com.aspose.tasks/pagelegend) - an instance of the [PageLegend](../../com.aspose.tasks/pagelegend) class which specifies rendering options of page legend.
### getMargins() {#getMargins--}
```
public final PageMargins getMargins()
```


ページ余白を指定する [PageMargins](../../com.aspose/tasks/pagemargins) クラスのインスタンスを取得します。

**Returns:**
[PageMargins](../../com.aspose.tasks/pagemargins) - an instance of the [PageMargins](../../com.aspose.tasks/pagemargins) class which specifies page margins.
### getName() {#getName--}
```
public final String getName()
```


設定データが使用されるビューの名前を取得します。

**Returns:**
java.lang.String - 設定データが使用されるビューの名前。
### getPageSettings() {#getPageSettings--}
```
public final PageSettings getPageSettings()
```


`PageSettings`([getPageSettings()](../../com.aspose/tasks/pageinfo\#getPageSettings--)) クラスのインスタンスを取得します。このクラスはページ印刷設定を指定します。

**Returns:**
[PageSettings](../../com.aspose.tasks/pagesettings) - an instance of the `PageSettings`([getPageSettings()](../../com.aspose.tasks/pageinfo\#getPageSettings--)) class which specifies page printing settings.
### getPageViewSettings() {#getPageViewSettings--}
```
public final PageViewSettings getPageViewSettings()
```


`PageViewSettings`([getPageViewSettings()](../../com.aspose/tasks/pageinfo\#getPageViewSettings--)) クラスのインスタンスを取得します。このクラスはページビュー印刷設定を指定します。

**Returns:**
[PageViewSettings](../../com.aspose.tasks/pageviewsettings) - an instance of the `PageViewSettings`([getPageViewSettings()](../../com.aspose.tasks/pageinfo\#getPageViewSettings--)) class which specifies page view printing settings.
### setFooter(HeaderFooterInfo value) {#setFooter-com.aspose.tasks.HeaderFooterInfo-}
```
public final void setFooter(HeaderFooterInfo value)
```


フッターデータを表す [HeaderFooterInfo](../../com.aspose/tasks/headerfooterinfo) クラスのインスタンスを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [HeaderFooterInfo](../../com.aspose.tasks/headerfooterinfo) | フッターデータを表す [HeaderFooterInfo](../../com.aspose/tasks/headerfooterinfo) クラスのインスタンス。 |

### setHeader(HeaderFooterInfo value) {#setHeader-com.aspose.tasks.HeaderFooterInfo-}
```
public final void setHeader(HeaderFooterInfo value)
```


ヘッダーデータを表す [HeaderFooterInfo](../../com.aspose/tasks/headerfooterinfo) クラスのインスタンスを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [HeaderFooterInfo](../../com.aspose.tasks/headerfooterinfo) | ヘッダーデータを表す [HeaderFooterInfo](../../com.aspose/tasks/headerfooterinfo) クラスのインスタンス。 |

### setLegend(PageLegend value) {#setLegend-com.aspose.tasks.PageLegend-}
```
public final void setLegend(PageLegend value)
```


ページ凡例の描画オプションを指定する [PageLegend](../../com.aspose/tasks/pagelegend) クラスのインスタンスを設定します。

--------------------

現在、ガントチャートビューにのみ適用されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [PageLegend](../../com.aspose.tasks/pagelegend) | ページ凡例の描画オプションを指定する [PageLegend](../../com.aspose/tasks/pagelegend) クラスのインスタンス。 |

