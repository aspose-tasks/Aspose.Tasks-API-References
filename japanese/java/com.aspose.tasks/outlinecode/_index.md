---
title: "OutlineCode"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "アウトライン コードの値を表します。"
type: docs
weight: 167
url: /ja/java/com.aspose.tasks/outlinecode/
---

**Inheritance:**
java.lang.Object
```
public class OutlineCode
```

アウトライン コードの値を表します。

--------------------

2つのデータが必要です - FieldIdで指定されるアウトラインコードテーブルへのポインタと、ValueIdまたはValueGuidで指定される値リストへのポインタです。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [OutlineCode()](#OutlineCode--) | 新しいインスタンスを初期化します。[OutlineCode](../../com.aspose.tasks/outlinecode) クラス。 |
| [OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue)](#OutlineCode-com.aspose.tasks.OutlineCodeDefinition-com.aspose.tasks.OutlineValue-) | 指定されたアウトラインコードとその値のいずれかを使用して、[OutlineCode](../../com.aspose.tasks/outlinecode) クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getFieldId()](#getFieldId--) | プロジェクトIDカスタムフィールドの数値を取得します。 |
| [getValueGuid()](#getValueGuid--) | 値リスト内の値のGUIDを取得します。 |
| [getValueId()](#getValueId--) | アウトラインコードコレクションの定義に関連付けられた、値リスト内のIdを取得します。 |
| [setFieldId(String value)](#setFieldId-java.lang.String-) | プロジェクトIDカスタムフィールドの数値を設定します。 |
| [setValueGuid(String value)](#setValueGuid-java.lang.String-) | 値リスト内の値のGUIDを設定します。 |
| [setValueId(int value)](#setValueId-int-) | アウトラインコードコレクションの定義に関連付けられた、値リスト内のIdを設定します。 |
### OutlineCode() {#OutlineCode--}
```
public OutlineCode()
```


新しいインスタンスを初期化します。[OutlineCode](../../com.aspose.tasks/outlinecode) クラス。

### OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue) {#OutlineCode-com.aspose.tasks.OutlineCodeDefinition-com.aspose.tasks.OutlineValue-}
```
public OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue)
```


指定されたアウトラインコードとその値のいずれかを使用して、[OutlineCode](../../com.aspose.tasks/outlinecode) クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| codeDefinition | [OutlineCodeDefinition](../../com.aspose.tasks/outlinecodedefinition) | アウトラインコード定義。 |
| outlineValue | [OutlineValue](../../com.aspose.tasks/outlinevalue) | アウトラインコード定義値の一つ。 |

### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


プロジェクトIDカスタムフィールドの数値を取得します。

**Returns:**
java.lang.String - プロジェクトIDカスタムフィールドの数値。
### getValueGuid() {#getValueGuid--}
```
public final String getValueGuid()
```


値リスト内の値のGUIDを取得します。ValueGuidは値リスト内のFieldGuidと一致します。

**Returns:**
java.lang.String - 値リスト内の値のGUID。
### getValueId() {#getValueId--}
```
public final int getValueId()
```


アウトラインコードコレクションの定義に関連付けられた、値リスト内のIdを取得します。

**Returns:**
int - アウトラインコードコレクションの定義に関連付けられた、値リスト内のId。
### setFieldId(String value) {#setFieldId-java.lang.String-}
```
public final void setFieldId(String value)
```


プロジェクトIDカスタムフィールドの数値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | プロジェクトIDカスタムフィールドの数値。 |

### setValueGuid(String value) {#setValueGuid-java.lang.String-}
```
public final void setValueGuid(String value)
```


値リスト内の値のGUIDを設定します。ValueGuidは値リスト内のFieldGuidと一致します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 値リスト内の値のGUID。 |

### setValueId(int value) {#setValueId-int-}
```
public final void setValueId(int value)
```


アウトラインコードコレクションの定義に関連付けられた、値リスト内のIdを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | アウトラインコードコレクションの定義に関連付けられた値リストの Id。 |

