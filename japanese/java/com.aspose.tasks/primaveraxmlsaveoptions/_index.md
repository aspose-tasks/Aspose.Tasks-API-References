---
title: "PrimaveraXmlSaveOptions"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "プロジェクトを Primavera xml フォーマットで保存する際に追加オプションを指定できます。"
type: docs
weight: 212
url: /ja/java/com.aspose.tasks/primaveraxmlsaveoptions/
---

**Inheritance:**
java.lang.Object、[com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class PrimaveraXmlSaveOptions extends SimpleSaveOptions
```

プロジェクトを Primavera xml フォーマットで保存する際に追加オプションを指定できます。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [PrimaveraXmlSaveOptions()](#PrimaveraXmlSaveOptions--) | 新しい[PrimaveraXmlSaveOptions](../../com.aspose.tasks/primaveraxmlsaveoptions)クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getSaveRootTask()](#getSaveRootTask--) | ルートタスクを保存するかどうかを示す値を取得します。 |
| [getSkipSummaryAssignments()](#getSkipSummaryAssignments--) | エクスポート時にリソースのサマリータスクへの割り当てをスキップすべきかどうかを示す値を取得します。 |
| [setSaveRootTask(boolean value)](#setSaveRootTask-boolean-) | ルートタスクを保存するかどうかを示す値を設定します。 |
| [setSkipSummaryAssignments(boolean value)](#setSkipSummaryAssignments-boolean-) | エクスポート時にリソースのサマリータスクへの割り当てをスキップすべきかどうかを示す値を設定します。 |
### PrimaveraXmlSaveOptions() {#PrimaveraXmlSaveOptions--}
```
public PrimaveraXmlSaveOptions()
```


新しい[PrimaveraXmlSaveOptions](../../com.aspose.tasks/primaveraxmlsaveoptions)クラスのインスタンスを初期化します。

### getSaveRootTask() {#getSaveRootTask--}
```
public final boolean getSaveRootTask()
```


ルートタスクを保存するかどうかを示す値を取得します。

**Returns:**
boolean - ルートタスクを保存するかどうかを示す値。
### getSkipSummaryAssignments() {#getSkipSummaryAssignments--}
```
public final boolean getSkipSummaryAssignments()
```


エクスポート時にリソースのサマリータスクへの割り当てをスキップすべきかどうかを示す値を取得します。

Primavera ソフトウェアはリソースをサマリー（WBS）タスクに割り当てることをサポートしていません。そのため、これらの割り当てをエクスポートすると、Primavera のモデルに従って無効なファイルになる可能性があります。true の場合、エクスポート時にサマリータスクへの割り当てはスキップされます。false（デフォルト値）の場合、エクスポート中にサマリータスクへの割り当てが検出されると例外がスローされます。

**Returns:**
boolean - エクスポート時にリソースのサマリータスクへの割り当てをスキップすべきかどうかを示す値。
### setSaveRootTask(boolean value) {#setSaveRootTask-boolean-}
```
public final void setSaveRootTask(boolean value)
```


ルートタスクを保存するかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | ルートタスクを保存するかどうかを示す値。 |

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

