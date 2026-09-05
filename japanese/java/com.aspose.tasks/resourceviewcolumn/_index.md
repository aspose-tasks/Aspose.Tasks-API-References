---
title: "ResourceViewColumn"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "ResourceUsage ビューと ResourceSheet ビューで使用される Projects ビュー クラス。"
type: docs
weight: 261
url: /ja/java/com.aspose.tasks/resourceviewcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public final class ResourceViewColumn extends ViewColumn
```

ResourceUsage ビューと ResourceSheet ビューで使用されるプロジェクトのビュー クラスです。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field)](#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-int-) | 新しい [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) クラスのインスタンスを初期化します。 |
| [ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter)](#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-) | 新しい [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) クラスのインスタンスを初期化します。 |
| [ResourceViewColumn(int width, int field)](#ResourceViewColumn-int-int-) | 新しい [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getColumnText(Resource resource)](#getColumnText-com.aspose.tasks.Resource-) | 現在のリソースを列テキストに変換します。 |
| [getField()](#getField--) | 列フィールドを返します。 |
| [setField(int value)](#setField-int-) | 列フィールドを設定します。 |
### ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field) {#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-int-}
```
public ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field)
```


新しい [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) クラスのインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | java.lang.String | 列の名前です。 |
| width | int | 列の幅（ピクセル単位）です。 |
| converter | [ResourceToColumnTextConverter](../../com.aspose.tasks/resourcetocolumntextconverter) | リソース データを列テキストに変換するコンバータ。 |
| フィールド | int | 列フィールド。 |

### ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter) {#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-}
```
public ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter)
```


新しい [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) クラスのインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | java.lang.String | 列の名前です。 |
| width | int | 列の幅（ピクセル単位）です。 |
| converter | [ResourceToColumnTextConverter](../../com.aspose.tasks/resourcetocolumntextconverter) | リソース データを列テキストに変換するコンバータ。 |

### ResourceViewColumn(int width, int field) {#ResourceViewColumn-int-int-}
```
public ResourceViewColumn(int width, int field)
```


新しい [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) クラスのインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| width | int | 列幅（ピクセル単位）。 |
| フィールド | int | 列フィールド。 |

### getColumnText(Resource resource) {#getColumnText-com.aspose.tasks.Resource-}
```
public final String getColumnText(Resource resource)
```


現在のリソースを列テキストに変換します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| resource | [Resource](../../com.aspose.tasks/resource) | 現在のリソースです。 |

**Returns:**
java.lang.String - 列テキストです。
### getField() {#getField--}
```
public int getField()
```


列フィールドを返します。 `Field`。

**Returns:**
int - 列フィールドの値です。
### setField(int value) {#setField-int-}
```
public void setField(int value)
```


列フィールドを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 列フィールドの値です。 |

