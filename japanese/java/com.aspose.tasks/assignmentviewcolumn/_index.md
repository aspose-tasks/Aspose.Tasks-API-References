---
title: "AssignmentViewColumn"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "プロジェクトビュー クラスです。"
type: docs
weight: 19
url: /ja/java/com.aspose.tasks/assignmentviewcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public class AssignmentViewColumn extends ViewColumn
```

プロジェクトのビュー クラスです。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter)](#AssignmentViewColumn-java.lang.String-int-com.aspose.tasks.AssignmentToColumnTextConverter-) | AssignmentViewColumn クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getColumnText(ResourceAssignment assignment)](#getColumnText-com.aspose.tasks.ResourceAssignment-) | 現在のリソース割り当てを列テキストに変換します。 |
| [getField()](#getField--) | 列フィールドを返します。 |
| [setField(int value)](#setField-int-) | 列フィールドを設定します。 |
### AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter) {#AssignmentViewColumn-java.lang.String-int-com.aspose.tasks.AssignmentToColumnTextConverter-}
```
public AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter)
```


AssignmentViewColumn クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | java.lang.String | 列の名前です。 |
| width | int | 列の幅（ピクセル単位）です。 |
| converter | [AssignmentToColumnTextConverter](../../com.aspose.tasks/assignmenttocolumntextconverter) | 割り当てデータを列テキストに変換するコンバータです。 |

### getColumnText(ResourceAssignment assignment) {#getColumnText-com.aspose.tasks.ResourceAssignment-}
```
public String getColumnText(ResourceAssignment assignment)
```


現在のリソース割り当てを列テキストに変換します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| assignment | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | 現在の割り当てです。 |

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

