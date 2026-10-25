---
title: "CustomProjectPropertyCollection"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "カスタム プロジェクト プロパティのコレクションを表します。"
type: docs
weight: 61
url: /ja/java/com.aspose.tasks/customprojectpropertycollection/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.PropertyCollection, com.aspose.tasks.PropertyKeyedCollection
```
public final class CustomProjectPropertyCollection extends PropertyKeyedCollection<CustomProjectProperty>
```

カスタム プロジェクト プロパティのコレクションを表します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [CustomProjectPropertyCollection()](#CustomProjectPropertyCollection--) | 新しいインスタンスを初期化します [CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection) クラス。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [add(String name, boolean value)](#add-java.lang.String-boolean-) | 新しいカスタムプロパティを作成します。 |
| [add(String name, double value)](#add-java.lang.String-double-) | 新しいカスタムプロパティを作成します。 |
| [add(String name, String value)](#add-java.lang.String-java.lang.String-) | 新しいカスタムプロパティを作成します。 |
| [add(String name, Date value)](#add-java.lang.String-java.util.Date-) | 新しいカスタムプロパティを作成します。 |
| [clear()](#clear--) | PropertyCollection をクリアします。 |
| [isReadOnly()](#isReadOnly--) | このコレクションが読み取り専用かどうかを示す値を取得します。そうでなければ false です。 |
| [remove(String name)](#remove-java.lang.String-) | 指定された名前のプロパティをコレクションから削除します。 |
### CustomProjectPropertyCollection() {#CustomProjectPropertyCollection--}
```
public CustomProjectPropertyCollection()
```


新しいインスタンスを初期化します [CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection) クラス。

### add(String name, boolean value) {#add-java.lang.String-boolean-}
```
public final CustomProjectProperty add(String name, boolean value)
```


新しいカスタムプロパティを作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | java.lang.String | プロパティの名前。 |
| 値 | boolean | 新しく作成されたプロパティオブジェクトの値。 |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, double value) {#add-java.lang.String-double-}
```
public final CustomProjectProperty add(String name, double value)
```


新しいカスタムプロパティを作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | java.lang.String | プロパティの名前。 |
| 値 | double | 新しく作成されたプロパティオブジェクトの値。 |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, String value) {#add-java.lang.String-java.lang.String-}
```
public final CustomProjectProperty add(String name, String value)
```


新しいカスタムプロパティを作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | java.lang.String | プロパティの名前。 |
| 値 | java.lang.String | 新しく作成されたプロパティオブジェクトの値。 |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, Date value) {#add-java.lang.String-java.util.Date-}
```
public final CustomProjectProperty add(String name, Date value)
```


新しいカスタムプロパティを作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | java.lang.String | プロパティの名前。 |
| 値 | java.util.Date | 新しく作成されたプロパティオブジェクトの値。 |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### clear() {#clear--}
```
public final void clear()
```


PropertyCollection をクリアします。

### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


このコレクションが読み取り専用かどうかを示す値を取得します。そうでなければ false です。

**Returns:**
boolean - このコレクションが読み取り専用かどうかを示す値。そうでなければ false。
### remove(String name) {#remove-java.lang.String-}
```
public final boolean remove(String name)
```


指定された名前のプロパティをコレクションから削除します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | java.lang.String | プロパティの大文字小文字を区別しない名前。 |

**Returns:**
boolean - 要素が正常に見つかり削除された場合は true、そうでない場合は false。
