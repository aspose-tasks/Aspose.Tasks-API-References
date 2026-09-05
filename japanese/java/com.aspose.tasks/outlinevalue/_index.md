---
title: "OutlineValue"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "アウトライン値を表します。"
type: docs
weight: 173
url: /ja/java/com.aspose.tasks/outlinevalue/
---

**Inheritance:**
java.lang.Object
```
public class OutlineValue
```

アウトライン値を表します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [OutlineValue()](#OutlineValue--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getDescription()](#getDescription--) | アウトライン値の説明を取得します。 |
| [getDurationValue()](#getDurationValue--) | タイプが Duration の場合、期間を取得します。 |
| [getParentValueId()](#getParentValueId--) | アウトラインコードの親ノードの ID を取得します。 |
| [getType()](#getType--) | アウトラインコードのタイプを取得します。 |
| [getValue()](#getValue--) | 実際の値を取得します。 |
| [getValueGuid()](#getValueGuid--) | プロジェクト全体で他の値と区別する GUID を取得します。 |
| [getValueId()](#getValueId--) | プロジェクト内のアウトラインコード値の一意の Id を取得します。 |
| [isCollapsed()](#isCollapsed--) | アウトライン値が折りたたまれているかどうかを示す値を取得します。 |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | アウトライン値が折りたたまれているかどうかを示す値を設定します。 |
| [setDescription(String value)](#setDescription-java.lang.String-) | アウトライン値の説明を設定します。 |
| [setDurationValue(Duration value)](#setDurationValue-com.aspose.tasks.Duration-) | タイプが Duration の場合、期間を設定します。 |
| [setParentValueId(int value)](#setParentValueId-int-) | アウトラインコードの親ノードの Id を設定します。 |
| [setType(int value)](#setType-int-) | アウトラインコードのタイプを設定します。 |
| [setValue(String value)](#setValue-java.lang.String-) | 実際の値を設定します。 |
| [setValueId(int value)](#setValueId-int-) | プロジェクト内のアウトラインコード値の一意の Id を設定します。 |
### OutlineValue() {#OutlineValue--}
```
public OutlineValue()
```


### getDescription() {#getDescription--}
```
public final String getDescription()
```


アウトライン値の説明を取得します。

**Returns:**
java.lang.String - アウトライン値の説明。
### getDurationValue() {#getDurationValue--}
```
public final Duration getDurationValue()
```


タイプが Duration の場合、期間を取得します。

--------------------

Duration タイプの OutlineValues の値を設定する必要がある場合は、`Value`([getValue()](../../com.aspose.tasks/outlinevalue\#getValue--)/[setValue(String)](../../com.aspose.tasks/outlinevalue\#setValue-String-)) よりもこのプロパティを使用してください。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the duration if Type is Duration.
### getParentValueId() {#getParentValueId--}
```
public final int getParentValueId()
```


アウトラインコードの親ノードの ID を取得します。

**Returns:**
int - アウトラインコードの親ノードの Id。
### getType() {#getType--}
```
public final int getType()
```


アウトラインコードのタイプを取得します。

**Returns:**
int - アウトラインコードのタイプ。
### getValue() {#getValue--}
```
public final String getValue()
```


実際の値を取得します。

**Returns:**
java.lang.String - 実際の値。
### getValueGuid() {#getValueGuid--}
```
public final UUID getValueGuid()
```


プロジェクト全体で他の値と区別する GUID を取得します。

**Returns:**
java.util.UUID - プロジェクト全体でこの値を他と区別する GUID。
### getValueId() {#getValueId--}
```
public final int getValueId()
```


プロジェクト内のアウトラインコード値の一意の Id を取得します。

**Returns:**
int - プロジェクト内のアウトラインコード値の一意の Id。
### isCollapsed() {#isCollapsed--}
```
public final boolean isCollapsed()
```


アウトライン値が折りたたまれているかどうかを示す値を取得します。

--------------------

これは MS Project 2010 の新しいプロパティです。

**Returns:**
boolean - アウトライン値が折りたたまれているかどうかを示す値。
### setCollapsed(boolean value) {#setCollapsed-boolean-}
```
public final void setCollapsed(boolean value)
```


アウトライン値が折りたたまれているかどうかを示す値を設定します。

--------------------

これは MS Project 2010 の新しいプロパティです。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | アウトライン値が折りたたまれているかどうかを示す値。 |

### setDescription(String value) {#setDescription-java.lang.String-}
```
public final void setDescription(String value)
```


アウトライン値の説明を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | アウトライン値の説明。 |

### setDurationValue(Duration value) {#setDurationValue-com.aspose.tasks.Duration-}
```
public final void setDurationValue(Duration value)
```


タイプが Duration の場合、期間を設定します。

--------------------

Duration タイプの OutlineValues の値を設定する必要がある場合は、`Value`([getValue()](../../com.aspose.tasks/outlinevalue\#getValue--)/[setValue(String)](../../com.aspose.tasks/outlinevalue\#setValue-String-)) よりもこのプロパティを使用してください。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | タイプが Duration の場合の期間。 |

### setParentValueId(int value) {#setParentValueId-int-}
```
public final void setParentValueId(int value)
```


アウトラインコードの親ノードの Id を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | アウトラインコードの親ノードの Id。 |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


アウトラインコードのタイプを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | アウトラインコードのタイプ。 |

### setValue(String value) {#setValue-java.lang.String-}
```
public final void setValue(String value)
```


実際の値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 実際の値。 |

### setValueId(int value) {#setValueId-int-}
```
public final void setValueId(int value)
```


プロジェクト内のアウトラインコード値の一意の Id を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | プロジェクト内のアウトラインコード値の一意の Id。 |

