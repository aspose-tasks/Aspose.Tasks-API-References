---
title: "ExtendedAttributeDefinition"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "プロジェクトに関連付けられた拡張属性定義を表します。"
type: docs
weight: 83
url: /ja/java/com.aspose.tasks/extendedattributedefinition/
---

**Inheritance:**
java.lang.Object
```
public class ExtendedAttributeDefinition
```

プロジェクトに関連付けられた拡張属性定義を表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [addLookupValue(Value value)](#addLookupValue-com.aspose.tasks.Value-) | 内部ルックアップリストに値を追加します。 |
| [compareTo(ExtendedAttributeDefinition o)](#compareTo-com.aspose.tasks.ExtendedAttributeDefinition-) | このオブジェクトを @\\{code ExtendedAttributeDefinition\\} クラスの別のインスタンスと比較します。 |
| [createExtendedAttribute()](#createExtendedAttribute--) | このオブジェクトのフィールド ID 値と等しいフィールド ID を持つ新しい拡張属性を作成します。 |
| [createExtendedAttribute(boolean flagValue)](#createExtendedAttribute-boolean-) | このオブジェクトのフィールド ID 値と等しいフィールド ID と、指定されたフラグ値を持つ新しい拡張属性を作成します。 |
| [createExtendedAttribute(Duration durationValue)](#createExtendedAttribute-com.aspose.tasks.Duration-) | このオブジェクトのフィールド ID 値と等しいフィールド ID と、指定された期間値を持つ新しい拡張属性を作成します。 |
| [createExtendedAttribute(Value lookupValue)](#createExtendedAttribute-com.aspose.tasks.Value-) | 指定された [Value](../../com.aspose.tasks/value) アイテムにリンクされた新しい拡張属性を作成します。 |
| [createExtendedAttribute(String textValue)](#createExtendedAttribute-java.lang.String-) | このオブジェクトのフィールド ID 値と等しいフィールド ID と、指定されたテキスト値を持つ新しい拡張属性を作成します。 |
| [createExtendedAttribute(BigDecimal numericValue)](#createExtendedAttribute-java.math.BigDecimal-) | このオブジェクトのフィールド ID 値と等しいフィールド ID と、指定された数値を持つ新しい拡張属性を作成します。 |
| [createExtendedAttribute(Date dateTimeValue)](#createExtendedAttribute-java.util.Date-) | このオブジェクトのフィールド ID 値と等しいフィールド ID と、指定された日付値を持つ新しい拡張属性を作成します。 |
| [createLookupResourceDefinition(int customFieldType, int fieldId, String alias)](#createLookupResourceDefinition-int-int-java.lang.String-) | ルックアップ付きの拡張属性定義を作成するファクトリーメソッドです。 |
| [createLookupResourceDefinition(int fieldId, String alias)](#createLookupResourceDefinition-int-java.lang.String-) | ルックアップ付きの拡張属性定義を作成するファクトリーメソッドです。 |
| [createLookupTaskDefinition(int customFieldType, int fieldId, String alias)](#createLookupTaskDefinition-int-int-java.lang.String-) | ルックアップ付きの拡張属性定義を作成するファクトリーメソッドです。 |
| [createLookupTaskDefinition(int fieldId, String alias)](#createLookupTaskDefinition-int-java.lang.String-) | ルックアップ付きの拡張属性定義を作成するファクトリーメソッドです。 |
| [createResourceDefinition(int customFieldType, int fieldId, String alias)](#createResourceDefinition-int-int-java.lang.String-) | Microsoft Project が "None" と表示するシンプルな拡張属性定義を作成するファクトリーメソッドです。 |
| [createResourceDefinition(int fieldId, String alias)](#createResourceDefinition-int-java.lang.String-) | Microsoft Project が "None" と表示するシンプルな拡張属性定義を作成するファクトリーメソッドです。 |
| [createTaskDefinition(int customFieldType, int fieldId, String alias)](#createTaskDefinition-int-int-java.lang.String-) | Microsoft Project が "None" と表示するシンプルな拡張属性定義を作成するファクトリーメソッドです。 |
| [createTaskDefinition(int fieldId, String alias)](#createTaskDefinition-int-java.lang.String-) | Microsoft Project が "None" と表示するシンプルな拡張属性定義を作成するファクトリーメソッドです。 |
| [equals(Object obj)](#equals-java.lang.Object-) | このインスタンスが指定されたオブジェクトと等しいかどうかを示すフラグを返します。 |
| [getAlias()](#getAlias--) | カスタム フィールドのエイリアスを取得します。 |
| [getAppendNewValues()](#getAppendNewValues--) | プロジェクトに追加された新しい値が自動的にリストに追加されるかどうかを示す値を取得します。 |
| [getAutoRollDown()](#getAutoRollDown--) | 割り当てへの自動ロールダウンが有効かどうかを示す値を取得します。 |
| [getCalculationType()](#getCalculationType--) | カスタム属性の値の計算タイプを取得します。 |
| [getCfType()](#getCfType--) | カスタム フィールドのタイプを取得します。 |
| [getDefault()](#getDefault--) | リスト内のデフォルト値を取得します。 |
| [getDefaultGuid()](#getDefaultGuid--) | デフォルト ルックアップ テーブル エントリの Guid を取得します。 |
| [getElementType()](#getElementType--) | 拡張属性がタスク、リソース、または割り当てに関連付けられているかどうかを取得します。 |
| [getFieldId()](#getFieldId--) | カスタム フィールドに対応するプロジェクト ID を取得します。 |
| [getFieldName()](#getFieldName--) | カスタム フィールドの名前を取得します。 |
| [getFormula()](#getFormula--) | Microsoft Project がカスタム タスク フィールドを設定するために使用する式を取得します。 |
| [getGraphicalIndicator()](#getGraphicalIndicator--) | 拡張属性に関連付けられたグラフィカル インジケータ情報を取得します。 |
| [getGuid()](#getGuid--) | カスタム フィールドの Guid を取得します。 |
| [getLookupUid()](#getLookupUid--) | カスタム フィールドに関連付けられたルックアップ テーブルの Guid を取得します。 |
| [getMaxMultiValues()](#getMaxMultiValues--) | ピックリストに設定できる最大値の数を取得します。 |
| [getParentProject()](#getParentProject--) | [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) インスタンスの親プロジェクトを取得します。 |
| [getPhoneticsAlias()](#getPhoneticsAlias--) | カスタム フィールドのエイリアスの発音（ふりがな）を取得します。 |
| [getRestrictValues()](#getRestrictValues--) | カスタム フィールドの値が `ValueList` の値に制限されているかどうかを示す値を取得します（`ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--))）。 |
| [getRollupType()](#getRollupType--) | ロールアップの計算方法を取得します。 |
| [getSecondaryGuid()](#getSecondaryGuid--) | 拡張属性のセカンダリ GUID を取得します。 |
| [getSecondaryPid()](#getSecondaryPid--) | カスタム フィールドのセカンダリ PID を取得します。 |
| [getSummaryRowsCalculationType()](#getSummaryRowsCalculationType--) | サマリ行のカスタム属性値の計算タイプを取得します。 |
| [getUserDef()](#getUserDef--) | カスタム フィールドがユーザー定義かどうかを示す値を取得します。 |
| [getValueList()](#getValueList--) | List&lt;Value&gt; ValueList を取得します。 |
| [getValuelistSortOrder()](#getValuelistSortOrder--) | 値リストの並び順を取得します。 |
| [hashCode()](#hashCode--) | インスタンスのハッシュコードを返します [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) クラス。 |
| [removeLookupValue(Value value)](#removeLookupValue-com.aspose.tasks.Value-) | 内部ルックアップリストから値を削除します。 |
| [setAlias(String value)](#setAlias-java.lang.String-) | カスタムフィールドのエイリアスを設定します。 |
| [setAppendNewValues(boolean value)](#setAppendNewValues-boolean-) | プロジェクトに追加された新しい値が自動的にリストに追加されるかどうかを示す値を設定します。 |
| [setAutoRollDown(boolean value)](#setAutoRollDown-boolean-) | 割り当てへの自動ロールダウンが有効かどうかを示す値を設定します。 |
| [setCalculationType(int value)](#setCalculationType-int-) | カスタム属性の値の計算タイプを設定します。 |
| [setDefault(String value)](#setDefault-java.lang.String-) | リスト内のデフォルト値を設定します。 |
| [setDefaultGuid(String value)](#setDefaultGuid-java.lang.String-) | デフォルトのルックアップテーブルエントリの Guid を設定します。 |
| [setElementType(int value)](#setElementType-int-) | 拡張属性がタスク、リソース、または割り当てに関連付けられているかを設定します。 |
| [setFieldId(String value)](#setFieldId-java.lang.String-) | カスタムフィールドのプロジェクト ID に対応するように設定します。 |
| [setFormula(String value)](#setFormula-java.lang.String-) | Microsoft Project がカスタムタスクフィールドを埋めるために使用する数式を設定します。 |
| [setGraphicalIndicator(GraphicalIndicatorsInfo value)](#setGraphicalIndicator-com.aspose.tasks.GraphicalIndicatorsInfo-) | 拡張属性に関連付けられたグラフィカルインジケータ情報を設定します。 |
| [setGuid(String value)](#setGuid-java.lang.String-) | カスタムフィールドの Guid を設定します。 |
| [setMaxMultiValues(int value)](#setMaxMultiValues-int-) | ピックリストに設定できる最大値の数を設定します。 |
| [setPhoneticsAlias(String value)](#setPhoneticsAlias-java.lang.String-) | カスタムフィールドのエイリアスの音声表記を設定します。 |
| [setRestrictValues(boolean value)](#setRestrictValues-boolean-) | カスタムフィールドの値が `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)) の値に制限されているかどうかを示す値を設定します。 |
| [setRollupType(int value)](#setRollupType-int-) | ロールアップの計算方法を設定します。 |
| [setSecondaryGuid(String value)](#setSecondaryGuid-java.lang.String-) | 拡張属性のセカンダリ GUID を設定します。 |
| [setSecondaryPid(String value)](#setSecondaryPid-java.lang.String-) | カスタムフィールドのセカンダリ PID を設定します。 |
| [setSummaryRowsCalculationType(int value)](#setSummaryRowsCalculationType-int-) | サマリ行のカスタム属性値の計算タイプを設定します。 |
| [setUserDef(boolean value)](#setUserDef-boolean-) | カスタムフィールドがユーザー定義かどうかを示す値を設定します。 |
| [setValuelistSortOrder(int value)](#setValuelistSortOrder-int-) | 値リストの並び順を設定します。 |
### addLookupValue(Value value) {#addLookupValue-com.aspose.tasks.Value-}
```
public final void addLookupValue(Value value)
```


内部ルックアップリストに値を追加します。これは `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)) を操作する推奨方法です。

--------------------

&gt; ```
&gt; このコードを使用してルックアップリストに新しい値を追加します:
&gt; ``````

taskTextAttr.addLookupValue(new Value() {{
this.setId(1);
this.setVal("Text value 1");
this.setDescription("Text value description 1");
}});
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Value](../../com.aspose.tasks/value) | Value to add into lookup.

--------------------

This method works only for [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) instances which have `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) equals to [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup). |

### compareTo(ExtendedAttributeDefinition o) {#compareTo-com.aspose.tasks.ExtendedAttributeDefinition-}
```
public int compareTo(ExtendedAttributeDefinition o)
```


Compares this object with another instance of the @\{code ExtendedAttributeDefinition\} class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) | the object to be compared. |

**Returns:**
int - a negative integer, zero, or a positive integer as this object is less than, equal to, or greater than the specified object.
### createExtendedAttribute() {#createExtendedAttribute--}
```
public final ExtendedAttribute createExtendedAttribute()
```


Creates a new extended attribute with the field ID which equals to this object's field ID value.

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(boolean flagValue) {#createExtendedAttribute-boolean-}
```
public final ExtendedAttribute createExtendedAttribute(boolean flagValue)
```


Creates a new extended attribute with the field ID which equals to this object's field ID value and the specified flag value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| flagValue | boolean | The specified flag value. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(Duration durationValue) {#createExtendedAttribute-com.aspose.tasks.Duration-}
```
public final ExtendedAttribute createExtendedAttribute(Duration durationValue)
```


Creates a new extended attribute with the field ID which equals to this object's field ID value and the specified duration value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| durationValue | [Duration](../../com.aspose.tasks/duration) | The specified duration value. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(Value lookupValue) {#createExtendedAttribute-com.aspose.tasks.Value-}
```
public final ExtendedAttribute createExtendedAttribute(Value lookupValue)
```


Creates new extended attribute linked with specified [Value](../../com.aspose.tasks/value) item.

--------------------

&gt; ```
&gt; Use this code to create new [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) using specific value:
&gt; ``````

 taskTextAttr.addLookupValue(value1);
 taskTextAttr.addLookupValue(value2);
 ExtendedAttribute extendedAttribute = taskTextAttr.createExtendedAttribute(value2);
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
|  | lookupValue | [Value](../../com.aspose.tasks/value) | 指定された[Value](../../com.aspose.tasks/value)項目。 |

--------------------

`lookupValue` は、[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) を使用して [addLookupValue(Value)](../../com.aspose.tasks/extendedattributedefinition\#addLookupValue-Value-) メソッドで事前に追加されている必要があります。 |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class linked with specified [Value](../../com.aspose.tasks/value) item.
### createExtendedAttribute(String textValue) {#createExtendedAttribute-java.lang.String-}
```
public final ExtendedAttribute createExtendedAttribute(String textValue)
```


このオブジェクトのフィールド ID 値と等しいフィールド ID と、指定されたテキスト値を持つ新しい拡張属性を作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| textValue | java.lang.String | 指定されたテキスト値。 |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(BigDecimal numericValue) {#createExtendedAttribute-java.math.BigDecimal-}
```
public final ExtendedAttribute createExtendedAttribute(BigDecimal numericValue)
```


このオブジェクトのフィールド ID 値と等しいフィールド ID と、指定された数値を持つ新しい拡張属性を作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| numericValue | java.math.BigDecimal | 指定された数値。 |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(Date dateTimeValue) {#createExtendedAttribute-java.util.Date-}
```
public final ExtendedAttribute createExtendedAttribute(Date dateTimeValue)
```


このオブジェクトのフィールド ID 値と等しいフィールド ID と、指定された日付値を持つ新しい拡張属性を作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| dateTimeValue | java.util.Date | 指定された日時値。 |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createLookupResourceDefinition(int customFieldType, int fieldId, String alias) {#createLookupResourceDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupResourceDefinition(int customFieldType, int fieldId, String alias)
```


ルックアップ付きの拡張属性定義を作成するファクトリーメソッドです。`CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) が [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup) に等しく、リソースでのみ使用できます。このメソッドを呼び出す際には `customFieldType`、`fieldId`、`alias` を指定する必要があります。

--------------------

&gt; ```
&gt; ルックアップ付きリソースのカスタムフィールド定義を作成し、テキスト値で埋める例を使用してください：
&gt; ``````

ExtendedAttributeDefinition resourceTextAttr = ExtendedAttributeDefinition.createLookupResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
resourceTextAttr.addLookupValue(new Value() {{
this.setId(1);
this.setVal("Text value 1");
this.setDescription("Text value description 1");
}});
resourceTextAttr.addLookupValue(new Value() {{
this.setId(2);
this.setVal("Text value 2");
this.setDescription("Text value description 2");
}});
project.getExtendedAttributes().add(resourceTextAttr);
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| customFieldType | int | The specified [CustomFieldType](../../com.aspose.tasks/customfieldtype) type. |
| fieldId | int | The specified [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource) field ID. |
| alias | java.lang.String | The specified String alias. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `customFieldType`, `fieldId` and `alias`.
### createLookupResourceDefinition(int fieldId, String alias) {#createLookupResourceDefinition-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupResourceDefinition(int fieldId, String alias)
```


Factory method which creates an extended attribute definition with lookup. It has `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) equals to [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup) and can be used in Resources only. You are required to specify `fieldId` and `alias` when call this method. The field type is inferred from field id.

--------------------

&gt; ```
&gt; Use this example to create a custom field definition for a resource with lookup and then fill it with text values:
&gt; ``````

 ExtendedAttributeDefinition resourceTextAttr = ExtendedAttributeDefinition.createLookupResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
     resourceTextAttr.addLookupValue(new Value() {{
         this.setId(1);
         this.setVal("Text value 1");
         this.setDescription("Text value description 1");
     }});
     resourceTextAttr.addLookupValue(new Value() {{
         this.setId(2);
         this.setVal("Text value 2");
         this.setDescription("Text value description 2");
     }});
     project.getExtendedAttributes().add(resourceTextAttr);
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fieldId | int | 指定された [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource) フィールド ID。 |
| alias | java.lang.String | 指定された String エイリアス。 |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createLookupTaskDefinition(int customFieldType, int fieldId, String alias) {#createLookupTaskDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupTaskDefinition(int customFieldType, int fieldId, String alias)
```


ルックアップ付きの拡張属性定義を作成するファクトリーメソッドです。`CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) が [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup) に等しく、Tasks のみで使用できます。このメソッドを呼び出す際には `customFieldType`、`fieldId`、`alias` を指定する必要があります。

--------------------

&gt; ```
&gt; この例を使用して、ルックアップ付きタスクのカスタムフィールド定義を作成し、テキスト値で埋めます：
&gt; ``````

ExtendedAttributeDefinition taskTextAttr = ExtendedAttributeDefinition.createLookupTaskDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
taskTextAttr.addLookupValue(new Value() {{
this.setId(1);
this.setVal("Text value 1");
this.setDescription("Text value description 1");
}});
taskTextAttr.addLookupValue(new Value() {{
this.setId(2);
this.setVal("Text value 2");
this.setDescription("Text value description 2");
}});
project.getExtendedAttributes().add(taskTextAttr);
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| customFieldType | int | The specified [CustomFieldType](../../com.aspose.tasks/customfieldtype) type. |
| fieldId | int | The specified [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) field ID. |
| alias | java.lang.String | The specified String alias. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `customFieldType`, `fieldId` and `alias`.
### createLookupTaskDefinition(int fieldId, String alias) {#createLookupTaskDefinition-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupTaskDefinition(int fieldId, String alias)
```


Factory method which creates an extended attribute definition with lookup. It has `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) equals to [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup) and can be used in Tasks only. You are required to specify `fieldId` and `alias` when call this method. The field type is inferred from field id.

--------------------

&gt; ```
&gt; Use this example to create a custom field definition for a task with lookup and then fill it with text values:
&gt; ``````

 ExtendedAttributeDefinition taskTextAttr = ExtendedAttributeDefinition.createLookupTaskDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
 taskTextAttr.addLookupValue(new Value() {{
     this.setId(1);
     this.setVal("Text value 1");
     this.setDescription("Text value description 1");
 }});
 taskTextAttr.addLookupValue(new Value() {{
     this.setId(2);
     this.setVal("Text value 2");
     this.setDescription("Text value description 2");
 }});
 project.getExtendedAttributes().add(taskTextAttr);
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fieldId | int | 指定された [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) フィールド ID。 |
| alias | java.lang.String | 指定された String エイリアス。 |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createResourceDefinition(int customFieldType, int fieldId, String alias) {#createResourceDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createResourceDefinition(int customFieldType, int fieldId, String alias)
```


シンプルな拡張属性定義を作成するファクトリーメソッドで、Microsoft Project では「None」と表示されます。`CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) が [CalculationType.None](../../com.aspose.tasks/calculationtype\#None) に等しく、Resource のみで使用できます。このメソッドを呼び出す際には `customFieldType`、`fieldId`、`alias` を指定する必要があります。

--------------------

&gt; ```
&gt; カスタムテキストフィールド定義を作成する例を使用してください：
&gt; ``````

ExtendedAttributeDefinition resourceTextAttr = ExtendedAttributeDefinition.createResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
project.getExtendedAttributes().add(resourceTextAttr);
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| customFieldType | int | The specified [CustomFieldType](../../com.aspose.tasks/customfieldtype) type. |
| fieldId | int | The specified [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource) field ID. |
| alias | java.lang.String | The specified String alias. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `customFieldType`, `fieldId` and `alias`.
### createResourceDefinition(int fieldId, String alias) {#createResourceDefinition-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createResourceDefinition(int fieldId, String alias)
```


Factory method which creates a simple extended attribute definition, which Microsoft Project shows as "None". It has `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) equals to [CalculationType.None](../../com.aspose.tasks/calculationtype\#None) and can be used in Resource only. You are required to specify `fieldId` and `alias` when call this method. The field type is inferred from field id.

--------------------

&gt; ```
&gt; Use this example to create a custom text field definition:
&gt; ``````

 ExtendedAttributeDefinition resourceTextAttr = ExtendedAttributeDefinition.createResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
 project.getExtendedAttributes().add(resourceTextAttr);
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fieldId | int | 指定された [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource) フィールド ID。 |
| alias | java.lang.String | 指定された String エイリアス。 |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createTaskDefinition(int customFieldType, int fieldId, String alias) {#createTaskDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createTaskDefinition(int customFieldType, int fieldId, String alias)
```


シンプルな拡張属性定義を作成するファクトリーメソッドで、Microsoft Project では「None」と表示されます。`CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) が [CalculationType.None](../../com.aspose.tasks/calculationtype\#None) に等しく、Tasks のみで使用できます。このメソッドを呼び出す際には `customFieldType`、`fieldId`、`alias` を指定する必要があります。

--------------------

&gt; ```
&gt; カスタムテキストフィールド定義を作成する例を使用してください：
&gt; ``````

ExtendedAttributeDefinition taskTextAttr = ExtendedAttributeDefinition.createTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
project.getExtendedAttributes().add(taskTextAttr);
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| customFieldType | int | The specified [CustomFieldType](../../com.aspose.tasks/customfieldtype) type. |
| fieldId | int | The specified [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) field ID. |
| alias | java.lang.String | The specified String alias. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `customFieldType`, `fieldId` and `alias`.
### createTaskDefinition(int fieldId, String alias) {#createTaskDefinition-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createTaskDefinition(int fieldId, String alias)
```


Factory method which creates a simple extended attribute definition, which Microsoft Project shows as "None". It has `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) equals to [CalculationType.None](../../com.aspose.tasks/calculationtype\#None) and can be used in Tasks only. You are required to specify `fieldId` and `alias` when calling this method. The field type is inferred from field id.

--------------------

&gt; ```
&gt; Use this example to create a custom text field definition:
&gt; ``````

 ExtendedAttributeDefinition taskTextAttr = ExtendedAttributeDefinition.createTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
 project.getExtendedAttributes().add(taskTextAttr);
 
```



**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fieldId | int | 指定された [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) フィールド ID。 |
| alias | java.lang.String | 指定された String エイリアス。 |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


このインスタンスが指定されたオブジェクトと等しいかどうかを示すフラグを返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| obj | java.lang.Object | このインスタンスと比較するために指定されたオブジェクト。 |

**Returns:**
boolean - このインスタンスが指定されたオブジェクトと等しいかどうかを示すフラグ。
### getAlias() {#getAlias--}
```
public final String getAlias()
```


カスタム フィールドのエイリアスを取得します。

**Returns:**
java.lang.String - カスタムフィールドのエイリアス。
### getAppendNewValues() {#getAppendNewValues--}
```
public final boolean getAppendNewValues()
```


プロジェクトに追加された新しい値が自動的にリストに追加されるかどうかを示す値を取得します。

--------------------

現在、MSP 2003/2007 Xml および MSP 2003 mpp 形式がサポートされています。

**Returns:**
boolean - プロジェクトに追加された新しい値が自動的にリストに追加されるかどうかを示す値。
### getAutoRollDown() {#getAutoRollDown--}
```
public final boolean getAutoRollDown()
```


割り当てへの自動ロールダウンが有効かどうかを示す値を取得します。

**Returns:**
boolean - 割り当てへの自動ロールダウンが有効かどうかを示す値。
### getCalculationType() {#getCalculationType--}
```
public final int getCalculationType()
```


カスタム属性の値の計算タイプを取得します。

**Returns:**
int - カスタム属性値の計算タイプ。
### getCfType() {#getCfType--}
```
public final int getCfType()
```


カスタム フィールドのタイプを取得します。

**Returns:**
int - カスタムフィールドのタイプ。
### getDefault() {#getDefault--}
```
public final String getDefault()
```


リスト内のデフォルト値を取得します。

--------------------

現在、MSP 2003/2007 Xml および MSP 2003 mpp 形式がサポートされています。

**Returns:**
java.lang.String - リスト内のデフォルト値です。
### getDefaultGuid() {#getDefaultGuid--}
```
public final String getDefaultGuid()
```


デフォルト ルックアップ テーブル エントリの Guid を取得します。

**Returns:**
java.lang.String - デフォルトのルックアップテーブルエントリの Guid です。
### getElementType() {#getElementType--}
```
public final int getElementType()
```


拡張属性がタスク、リソース、または割り当てに関連付けられているかどうかを取得します。

**Returns:**
int - 拡張属性はタスク、リソース、または割り当てに関連付けられます。
### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


取得はカスタム フィールドのプロジェクト ID に対応します。`FieldId`（[getFieldId()](../../com.aspose.tasks/extendedattributedefinition\#getFieldId--) / [setFieldId(String)](../../com.aspose.tasks/extendedattributedefinition\#setFieldId-String-)）プロパティを指定するには、[ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) クラスの定数の文字列表現を使用します。

--------------------

&gt; ```
&gt;
&gt; ``````

customFieldDefinition.setFieldId(Integer.toString(ExtendedAttributeTask.Number10));
 
```

--------------------

Preferable way to set `FieldId`([getFieldId()](../../com.aspose.tasks/extendedattributedefinition\#getFieldId--)/ [setFieldId(String)](../../com.aspose.tasks/extendedattributedefinition\#setFieldId-String-)) property is to create [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) using one of the dedicated factory methods like [createTaskDefinition(int, String)](../../com.aspose.tasks/extendedattributedefinition\#createTaskDefinition-int--String-) or [createLookupTaskDefinition(int, int, String)](../../com.aspose.tasks/extendedattributedefinition\#createLookupTaskDefinition-int--int--String-).

**Returns:**
java.lang.String - corresponds to the project id of a custom field.
### getFieldName() {#getFieldName--}
```
public final String getFieldName()
```


Gets the name of a custom field.

--------------------

Should not be set directly, instead create ExtendedAttributeDefinition using strongly typed static factory methods named like create\*Definition().

**Returns:**
java.lang.String - the name of a custom field.
### getFormula() {#getFormula--}
```
public final String getFormula()
```


Gets the formula that Microsoft Project uses to populate a custom task field.

**Returns:**
java.lang.String - the formula that Microsoft Project uses to populate a custom task field.
### getGraphicalIndicator() {#getGraphicalIndicator--}
```
public final GraphicalIndicatorsInfo getGraphicalIndicator()
```


Gets a graphical indicators info associated with the extended attribute. Applicable to MPP format.

**Returns:**
[GraphicalIndicatorsInfo](../../com.aspose.tasks/graphicalindicatorsinfo) - a graphical indicators info associated with the extended attribute.
### getGuid() {#getGuid--}
```
public final String getGuid()
```


Gets the Guid of a custom field.

--------------------

Currently supported for Xml format only.

**Returns:**
java.lang.String - the Guid of a custom field.
### getLookupUid() {#getLookupUid--}
```
public final String getLookupUid()
```


Gets a Guid of the lookup table associated with a custom field.

--------------------

In order to create a custom field with lookup, use one of the factory methods: [createLookupTaskDefinition(int, int, String)](../../com.aspose.tasks/extendedattributedefinition\#createLookupTaskDefinition-int--int--String-) or [createLookupResourceDefinition(int, int, String)](../../com.aspose.tasks/extendedattributedefinition\#createLookupResourceDefinition-int--int--String-).

**Returns:**
java.lang.String - a Guid of the lookup table associated with a custom field.
### getMaxMultiValues() {#getMaxMultiValues--}
```
public final int getMaxMultiValues()
```


Gets the maximum number of values you can set in a pick list.

--------------------

Currently supported for Xml format only.

**Returns:**
int - the maximum number of values you can set in a pick list.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Gets the parent project for the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) instance.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project for the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) instance.
### getPhoneticsAlias() {#getPhoneticsAlias--}
```
public final String getPhoneticsAlias()
```


Gets the phonetic pronunciation of the alias of a custom field.

--------------------

Currently supported for Xml format only.

**Returns:**
java.lang.String - the phonetic pronunciation of the alias of a custom field.
### getRestrictValues() {#getRestrictValues--}
```
public final boolean getRestrictValues()
```


Gets a value indicating whether the custom field values are restricted to values in the `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)).

**Returns:**
boolean - a value indicating whether the custom field values are restricted to values in the `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)).
### getRollupType() {#getRollupType--}
```
public final int getRollupType()
```


Gets the way rollups are calculated.

--------------------

Writing currently supported for Xml format only.

**Returns:**
int - the way rollups are calculated.
### getSecondaryGuid() {#getSecondaryGuid--}
```
public final String getSecondaryGuid()
```


Gets the secondary guid of extended attribute.

--------------------

This is new for MS Project 2010 property.

**Returns:**
java.lang.String - the secondary guid of extended attribute.
### getSecondaryPid() {#getSecondaryPid--}
```
public final String getSecondaryPid()
```


Gets the secondary PID of a custom field.

**Returns:**
java.lang.String - the secondary PID of a custom field.
### getSummaryRowsCalculationType() {#getSummaryRowsCalculationType--}
```
public final int getSummaryRowsCalculationType()
```


Gets the type of calculation of the custom attribute's value for summary rows.

**Returns:**
int - the type of calculation of the custom attribute's value for summary rows.
### getUserDef() {#getUserDef--}
```
public final boolean getUserDef()
```


Gets a value indicating whether a custom field is user defined.

--------------------

Currently supported for Xml format only.

**Returns:**
boolean - a value indicating whether a custom field is user defined.
### getValueList() {#getValueList--}
```
public final List<Value> getValueList()
```


Gets the List&lt;Value&gt; ValueList.

--------------------

When values of extended attributes are specified as properties of elements in the schema, they may either be specified by values or by references to the values contained in this list. Applications may assume ordering of the list by ordering specified here. Currently supported for MSP 2003/2007 Xml and MSP 2003 mpp formats. Do not change this list directly. Use ExtendedAttributeDefinition.addLookupValue/removeLookupValue methods instead.

**Returns:**
java.util.List&lt;com.aspose.tasks.Value&gt; - the List&lt;Value&gt; ValueList.
### getValuelistSortOrder() {#getValuelistSortOrder--}
```
public final int getValuelistSortOrder()
```


Gets the way value lists are sorted. Values are: 0=Descending, 1=Ascending.

--------------------

Currently supported for MSP 2003/2007 Xml and MSP 2003 mpp formats.

**Returns:**
int - the way value lists are sorted.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Returns a hash code for the instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class.

**Returns:**
int - a hash code for this object.
### removeLookupValue(Value value) {#removeLookupValue-com.aspose.tasks.Value-}
```
public final void removeLookupValue(Value value)
```


Removes a value from the internal lookup list. This is a preferable way for manipulations with the `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Value](../../com.aspose.tasks/value) | Value to remove from lookup.

--------------------

This method works only for [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) instances which have `CalculationType`([getCalculationType](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) equals to [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup). |

### setAlias(String value) {#setAlias-java.lang.String-}
```
public final void setAlias(String value)
```


Sets the alias of a custom field.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the alias of a custom field. |

### setAppendNewValues(boolean value) {#setAppendNewValues-boolean-}
```
public final void setAppendNewValues(boolean value)
```


Sets a value indicating whether new values added to a project are automatically added to the list.

--------------------

Currently supported for MSP 2003/2007 Xml and MSP 2003 mpp formats.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether new values added to a project are automatically added to the list. |

### setAutoRollDown(boolean value) {#setAutoRollDown-boolean-}
```
public final void setAutoRollDown(boolean value)
```


Sets a value indicating whether an automatic roll down to assignments is enabled.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether an automatic roll down to assignments is enabled. |

### setCalculationType(int value) {#setCalculationType-int-}
```
public final void setCalculationType(int value)
```


Sets the type of calculation of the custom attribute's value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the type of calculation of the custom attribute's value. |

### setDefault(String value) {#setDefault-java.lang.String-}
```
public final void setDefault(String value)
```


Sets the default value in the list.

Currently supported for MSP 2003/2007 Xml and MSP 2003 mpp formats.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the default value in the list. |

### setDefaultGuid(String value) {#setDefaultGuid-java.lang.String-}
```
public final void setDefaultGuid(String value)
```


Sets the Guid of the default lookup table entry.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the Guid of the default lookup table entry. |

### setElementType(int value) {#setElementType-int-}
```
public final void setElementType(int value)
```


Sets the extended attribute is associated with a task, a resource or an assignment.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the extended attribute is associated with a task, a resource or an assignment. |

### setFieldId(String value) {#setFieldId-java.lang.String-}
```
public final void setFieldId(String value)
```


Sets corresponds to the project id of a custom field. Use string representation of a constant from [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) class to specify `FieldId`([getFieldId()](../../com.aspose.tasks/extendedattributedefinition\#getFieldId--)/ [setFieldId(String)](../../com.aspose.tasks/extendedattributedefinition\#setFieldId-String-)) property.

--------------------

&gt; ```
&gt; 
&gt; ``````

 customFieldDefinition.setFieldId(Integer.toString(ExtendedAttributeTask.Number10));
 
```

--------------------

Preferable way to set `FieldId`([getFieldId()](../../com.aspose/tasks/extendedattributedefinition\#getFieldId--)/ [setFieldId(String)](../../com.aspose/tasks/extendedattributedefinition\#setFieldId-String-)) property is to create [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) using one of the dedicated factory methods like [createTaskDefinition(int, String)](../../com.aspose.tasks/extendedattributedefinition\#createTaskDefinition-int--String-) or [createLookupTaskDefinition(int, int, String)](../../com.aspose.tasks/extendedattributedefinition\#createLookupTaskDefinition-int--int--String-).

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | カスタム フィールドのプロジェクト ID に対応します。 |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public final void setFormula(String value)
```


Microsoft Project がカスタムタスクフィールドを埋めるために使用する数式を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | Microsoft Project がカスタム タスク フィールドを入力するために使用する数式です。 |

### setGraphicalIndicator(GraphicalIndicatorsInfo value) {#setGraphicalIndicator-com.aspose.tasks.GraphicalIndicatorsInfo-}
```
public final void setGraphicalIndicator(GraphicalIndicatorsInfo value)
```


拡張属性に関連付けられたグラフィカル インジケータ情報を設定します。MPP 形式に適用可能です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [GraphicalIndicatorsInfo](../../com.aspose.tasks/graphicalindicatorsinfo) | 拡張属性に関連付けられたグラフィカル インジケータ情報。 |

### setGuid(String value) {#setGuid-java.lang.String-}
```
public final void setGuid(String value)
```


カスタムフィールドの Guid を設定します。

--------------------

現在、Xml 形式のみサポートされています。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | カスタム フィールドの Guid です。 |

### setMaxMultiValues(int value) {#setMaxMultiValues-int-}
```
public final void setMaxMultiValues(int value)
```


ピックリストに設定できる最大値の数を設定します。

--------------------

現在、Xml 形式のみサポートされています。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | ピックリストに設定できる最大値の数です。 |

### setPhoneticsAlias(String value) {#setPhoneticsAlias-java.lang.String-}
```
public final void setPhoneticsAlias(String value)
```


カスタムフィールドのエイリアスの音声表記を設定します。

--------------------

現在、Xml 形式のみサポートされています。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | カスタム フィールドのエイリアスの音声表記です。 |

### setRestrictValues(boolean value) {#setRestrictValues-boolean-}
```
public final void setRestrictValues(boolean value)
```


カスタムフィールドの値が `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)) の値に制限されているかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | カスタム フィールドの値が以下の値に制限されているかどうかを示す値 |

### setRollupType(int value) {#setRollupType-int-}
```
public final void setRollupType(int value)
```


ロールアップの計算方法を設定します。

--------------------

書き込みは現在、Xml 形式のみサポートされています。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | ロールアップの計算方法です。 |

### setSecondaryGuid(String value) {#setSecondaryGuid-java.lang.String-}
```
public final void setSecondaryGuid(String value)
```


拡張属性のセカンダリ GUID を設定します。

--------------------

これは MS Project 2010 の新しいプロパティです。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 拡張属性のセカンダリ GUID です。 |

### setSecondaryPid(String value) {#setSecondaryPid-java.lang.String-}
```
public final void setSecondaryPid(String value)
```


カスタムフィールドのセカンダリ PID を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | カスタム フィールドのセカンダリ PID です。 |

### setSummaryRowsCalculationType(int value) {#setSummaryRowsCalculationType-int-}
```
public final void setSummaryRowsCalculationType(int value)
```


サマリ行のカスタム属性値の計算タイプを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | サマリ行のカスタム属性値の計算タイプです。 |

### setUserDef(boolean value) {#setUserDef-boolean-}
```
public final void setUserDef(boolean value)
```


カスタムフィールドがユーザー定義かどうかを示す値を設定します。

--------------------

現在、Xml 形式のみサポートされています。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | カスタム フィールドがユーザー定義かどうかを示す値です。 |

### setValuelistSortOrder(int value) {#setValuelistSortOrder-int-}
```
public final void setValuelistSortOrder(int value)
```


値リストのソート方法を設定します。値は: 0=降順、1=昇順です。

--------------------

現在、MSP 2003/2007 Xml および MSP 2003 mpp 形式がサポートされています。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 値リストの並び順。 |

