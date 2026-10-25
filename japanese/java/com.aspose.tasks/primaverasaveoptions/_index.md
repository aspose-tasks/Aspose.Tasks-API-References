---
title: "PrimaveraSaveOptions"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "プロジェクトを Primavera XER フォーマットで保存する際に追加オプションを指定できます。"
type: docs
weight: 208
url: /ja/java/com.aspose.tasks/primaverasaveoptions/
---

**Inheritance:**
java.lang.Object、[com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class PrimaveraSaveOptions extends SimpleSaveOptions
```

プロジェクトを Primavera XER フォーマットで保存する際に追加オプションを指定できます。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [PrimaveraSaveOptions()](#PrimaveraSaveOptions--) | 新しい [PrimaveraSaveOptions](../../com.aspose.tasks/primaverasaveoptions) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getActivityIdIncrement()](#getActivityIdIncrement--) | アクティビティ ID の再番号付けに使用される増分を取得します。 |
| [getActivityIdPrefix()](#getActivityIdPrefix--) | アクティビティ ID の再番号付けに使用されるプレフィックスを取得します。 |
| [getActivityIdSuffix()](#getActivityIdSuffix--) | アクティビティ ID の再番号付けに使用されるサフィックスを取得します。 |
| [getRenumberActivityIds()](#getRenumberActivityIds--) | アクティビティ ID を再番号付けする必要があるかどうかを示す値を取得します。 |
| [getSkipSummaryAssignments()](#getSkipSummaryAssignments--) | エクスポート時にリソースのサマリータスクへの割り当てをスキップすべきかどうかを示す値を取得します。 |
| [setActivityIdIncrement(int value)](#setActivityIdIncrement-int-) | アクティビティ ID の再番号付けに使用される増分を設定します。 |
| [setActivityIdPrefix(String value)](#setActivityIdPrefix-java.lang.String-) | アクティビティ ID の再番号付けに使用されるプレフィックスを設定します。 |
| [setActivityIdSuffix(int value)](#setActivityIdSuffix-int-) | アクティビティ ID の再番号付けに使用されるサフィックスを設定します。 |
| [setRenumberActivityIds(boolean value)](#setRenumberActivityIds-boolean-) | アクティビティ ID を再番号付けする必要があるかどうかを示す値を設定します。 |
| [setSkipSummaryAssignments(boolean value)](#setSkipSummaryAssignments-boolean-) | エクスポート時にリソースのサマリータスクへの割り当てをスキップすべきかどうかを示す値を設定します。 |
### PrimaveraSaveOptions() {#PrimaveraSaveOptions--}
```
public PrimaveraSaveOptions()
```


新しい [PrimaveraSaveOptions](../../com.aspose.tasks/primaverasaveoptions) クラスのインスタンスを初期化します。

### getActivityIdIncrement() {#getActivityIdIncrement--}
```
public final int getActivityIdIncrement()
```


アクティビティ ID の再番号付けに使用される増分を取得します。

**Returns:**
int - アクティビティ ID の再番号付けに使用される増分。
### getActivityIdPrefix() {#getActivityIdPrefix--}
```
public final String getActivityIdPrefix()
```


アクティビティ ID の再番号付けに使用されるプレフィックスを取得します。

**Returns:**
java.lang.String - アクティビティ ID の再番号付けに使用されるプレフィックス。
### getActivityIdSuffix() {#getActivityIdSuffix--}
```
public final int getActivityIdSuffix()
```


アクティビティ ID の再番号付けに使用されるサフィックスを取得します。

**Returns:**
int - アクティビティ ID の再番号付けに使用されるサフィックス。
### getRenumberActivityIds() {#getRenumberActivityIds--}
```
public final boolean getRenumberActivityIds()
```


アクティビティ ID を再番号付けする必要があるかどうかを示す値を取得します。

**Returns:**
boolean - アクティビティ ID を再番号付けする必要があるかどうかを示す値。
### getSkipSummaryAssignments() {#getSkipSummaryAssignments--}
```
public final boolean getSkipSummaryAssignments()
```


エクスポート時にリソースのサマリータスクへの割り当てをスキップすべきかどうかを示す値を取得します。

Primavera ソフトウェアはリソースをサマリー（WBS）タスクに割り当てることをサポートしていません。そのため、これらの割り当てをエクスポートすると、Primavera のモデルに従って無効なファイルになる可能性があります。true の場合、エクスポート時にサマリータスクへの割り当てはスキップされます。false（デフォルト値）の場合、エクスポート中にサマリータスクへの割り当てが検出されると例外がスローされます。

**Returns:**
boolean - エクスポート時にリソースのサマリータスクへの割り当てをスキップすべきかどうかを示す値。
### setActivityIdIncrement(int value) {#setActivityIdIncrement-int-}
```
public final void setActivityIdIncrement(int value)
```


アクティビティ ID の再番号付けに使用される増分を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | アクティビティ ID の再番号付けに使用される増分。 |

### setActivityIdPrefix(String value) {#setActivityIdPrefix-java.lang.String-}
```
public final void setActivityIdPrefix(String value)
```


アクティビティ ID の再番号付けに使用されるプレフィックスを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | アクティビティ ID の再番号付けに使用されるプレフィックス。 |

### setActivityIdSuffix(int value) {#setActivityIdSuffix-int-}
```
public final void setActivityIdSuffix(int value)
```


アクティビティ ID の再番号付けに使用されるサフィックスを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | アクティビティ ID の再番号付けに使用されるサフィックス。 |

### setRenumberActivityIds(boolean value) {#setRenumberActivityIds-boolean-}
```
public final void setRenumberActivityIds(boolean value)
```


アクティビティ ID を再番号付けする必要があるかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | アクティビティ ID を再番号付けする必要があるかどうかを示す値。 |

### setSkipSummaryAssignments(boolean value) {#setSkipSummaryAssignments-boolean-}
```
public final void setSkipSummaryAssignments(boolean value)
```


エクスポート時にリソースのサマリータスクへの割り当てをスキップすべきかどうかを示す値を設定します。

Primavera ソフトウェアはリソースをサマリー（WBS）タスクに割り当てることをサポートしていません。そのため、これらの割り当てをエクスポートすると、Primavera のモデルに従って無効なファイルになる可能性があります。true の場合、エクスポート時にサマリータスクへの割り当てはスキップされます。false（デフォルト値）の場合、エクスポート中にサマリータスクへの割り当てが検出されると例外がスローされます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | エクスポート時にリソースのサマリータスクへの割り当てをスキップすべきかどうかを示す値。 |

