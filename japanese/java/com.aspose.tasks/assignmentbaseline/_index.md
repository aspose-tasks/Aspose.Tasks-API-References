---
title: "AssignmentBaseline"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "リソース割り当てのベースラインを表します。"
type: docs
weight: 17
url: /ja/java/com.aspose.tasks/assignmentbaseline/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.Baseline](../../com.aspose.tasks/baseline)
```
public class AssignmentBaseline extends Baseline
```

リソース割り当てのベースラインを表します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [AssignmentBaseline()](#AssignmentBaseline--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [compareTo(AssignmentBaseline other)](#compareTo-com.aspose.tasks.AssignmentBaseline-) | IComparable インターフェイスの実装。 |
| [equals(AssignmentBaseline other)](#equals-com.aspose.tasks.AssignmentBaseline-) | このインスタンスが指定された AssignmentBaseline オブジェクトと等しいかどうかを示す値を返します。 |
| [equals(Object obj)](#equals-java.lang.Object-) | このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。 |
| [getFinish()](#getFinish--) | ベースラインが保存されたときのリソース割り当ての予定完了日を取得します。 |
| [getStart()](#getStart--) | ベースラインが保存されたときのリソース割り当ての予定開始日を取得します。 |
| [getTimephasedData()](#getTimephasedData--) | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) のインスタンスを取得します。 |
| [hashCode()](#hashCode--) | この AssignmentBaseline のハッシュコード値を返します。 |
| [setFinish(Date value)](#setFinish-java.util.Date-) | ベースラインが保存されたときのリソース割り当ての予定完了日を設定します。 |
| [setStart(Date value)](#setStart-java.util.Date-) | ベースラインが保存されたときのリソース割り当ての予定開始日を設定します。 |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | このオブジェクトの [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) インスタンスを設定します。 |
### AssignmentBaseline() {#AssignmentBaseline--}
```
public AssignmentBaseline()
```


### compareTo(AssignmentBaseline other) {#compareTo-com.aspose.tasks.AssignmentBaseline-}
```
public final int compareTo(AssignmentBaseline other)
```


IComparable インターフェイスの実装です。このインスタンスを指定された Baseline オブジェクトと比較します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| other | [AssignmentBaseline](../../com.aspose.tasks/assignmentbaseline) | このインスタンスと比較するための指定された Baseline オブジェクト。 |

**Returns:**
int - このインスタンスが指定されたオブジェクトより小さい場合は -1、指定されたオブジェクトより大きい場合は 1 を返し、それ以外の場合は 0 を返します。
### equals(AssignmentBaseline other) {#equals-com.aspose.tasks.AssignmentBaseline-}
```
public final boolean equals(AssignmentBaseline other)
```


このインスタンスが指定された AssignmentBaseline オブジェクトと等しいかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| other | [AssignmentBaseline](../../com.aspose.tasks/assignmentbaseline) | このインスタンスと比較するための指定された AssignmentBaseline オブジェクトです。 |

**Returns:**
boolean - このインスタンスが指定された AssignmentBaseline オブジェクトと等しい場合は true を返し、そうでない場合は false を返します。
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| obj | java.lang.Object | このインスタンスと比較するための指定されたオブジェクト。 |

**Returns:**
boolean - このインスタンスが指定されたオブジェクトと等しい場合は true を返し、そうでない場合は false を返します。
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


ベースラインが保存されたときのリソース割り当ての予定完了日を取得します。

値: このベースラインが保存されたときのリソース割り当ての完了日。

**Returns:**
java.util.Date - ベースラインが保存されたときのリソース割り当ての予定完了日。
### getStart() {#getStart--}
```
public final Date getStart()
```


ベースラインが保存されたときのリソース割り当ての予定開始日を取得します。

値: このベースラインが保存されたときのリソース割り当ての開始日。

**Returns:**
java.util.Date - ベースラインが保存されたときのリソース割り当ての予定開始日。
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


このオブジェクトの [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) インスタンスを取得します。リソース割り当てベースラインに関連付けられた時間フェーズデータです。

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) instance for this object. Value: The collection of Time phased data associated with this baseline.
### hashCode() {#hashCode--}
```
public int hashCode()
```


この AssignmentBaseline のハッシュコード値を返します。

**Returns:**
int - このオブジェクトのハッシュコード値を返します。
### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


ベースラインが保存されたときのリソース割り当ての予定完了日を設定します。

値: このベースラインが保存されたときのリソース割り当ての完了日。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | ベースラインが保存されたときのリソース割り当ての予定完了日。 |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


ベースラインが保存されたときのリソース割り当ての予定開始日を設定します。

値: このベースラインが保存されたときのリソース割り当ての開始日。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | ベースラインが保存されたときのリソース割り当ての予定開始日。 |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


このオブジェクトの [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) インスタンスを設定します。リソース割り当てベースラインに関連付けられた時間フェーズデータです。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | このオブジェクトの [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) インスタンス。 |

