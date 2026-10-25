---
title: "LevelingOptions"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "リソース平準化のパラメータを指定できます。"
type: docs
weight: 142
url: /ja/java/com.aspose.tasks/levelingoptions/
---

**Inheritance:**
java.lang.Object
```
public final class LevelingOptions
```

リソース平準化のパラメータを指定できます。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [LevelingOptions()](#LevelingOptions--) | 新しい [LevelingOptions](../../com.aspose/tasks/levelingoptions) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getCancellationToken()](#getCancellationToken--) | プロジェクトのレベリング操作をキャンセルするために使用できるトークンを取得します。 |
| [getFinishDate()](#getFinishDate--) | レベリング期間の終了日を取得します。 |
| [getLevelingOrder()](#getLevelingOrder--) | レベリングアルゴリズムが過剰割り当てのあるタスクを遅延させる順序を取得します。 |
| [getMessageHandler()](#getMessageHandler--) | リソースレベリング中に Aspose.Tasks が生成するログメッセージをインターセプトできるメッセージハンドラコールバックを取得します。 |
| [getMessageLevel()](#getMessageLevel--) | リソースレベリング中に Aspose.Tasks が出力するログメッセージのレベルを取得します。 |
| [getResources()](#getResources--) | レベリング対象となるリソースの一覧を取得します。 |
| [getStartDate()](#getStartDate--) | レベリング期間の開始日を取得します。 |
| [setCancellationToken(CancellationToken value)](#setCancellationToken-com.aspose.tasks.CancellationToken-) | プロジェクトのレベリング操作をキャンセルするために使用できるトークンを設定します。 |
| [setFinishDate(Date value)](#setFinishDate-java.util.Date-) | レベリング期間の終了日を設定します。 |
| [setLevelingOrder(int value)](#setLevelingOrder-int-) | レベリングアルゴリズムが過剰割り当てのあるタスクを遅延させる順序。 |
| [setMessageHandler(IMessageHandler value)](#setMessageHandler-com.aspose.tasks.IMessageHandler-) | リソースレベリング中に Aspose.Tasks が生成するログメッセージをインターセプトできるメッセージハンドラコールバックを設定します。 |
| [setMessageLevel(int value)](#setMessageLevel-int-) | リソースレベリング中に Aspose.Tasks が出力するログメッセージのレベルを設定します。 |
| [setResources(List&lt;Resource&gt; value)](#setResources-java.util.List-com.aspose.tasks.Resource--) | レベリング対象となるリソースの一覧を設定します。 |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | レベリング期間の開始日を設定します。 |
### LevelingOptions() {#LevelingOptions--}
```
public LevelingOptions()
```


新しい [LevelingOptions](../../com.aspose/tasks/levelingoptions) クラスのインスタンスを初期化します。

### getCancellationToken() {#getCancellationToken--}
```
public final CancellationToken getCancellationToken()
```


プロジェクトのレベリング操作をキャンセルするために使用できるトークンを取得します。

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token which can be used to cancel a project leveling operation.
### getFinishDate() {#getFinishDate--}
```
public final Date getFinishDate()
```


レベリング期間の終了日を取得します。デフォルト値はプロジェクトの完了日です。

**Returns:**
java.util.Date - レベリング期間の終了日。
### getLevelingOrder() {#getLevelingOrder--}
```
public final int getLevelingOrder()
```


レベリングアルゴリズムが過剰割り当てのあるタスクを遅延させる順序を取得します。過剰割り当てを引き起こすタスクと遅延可能なタスクを特定した後、どのタスクを最初に遅延させるかを指定された順序で使用します。

**Returns:**
int - レベリングアルゴリズムが過剰割り当てのあるタスクを遅延させる順序。
### getMessageHandler() {#getMessageHandler--}
```
public final IMessageHandler getMessageHandler()
```


リソースレベリング中に Aspose.Tasks が生成するログメッセージをインターセプトできるメッセージハンドラコールバックを取得します。

**Returns:**
[IMessageHandler](../../com.aspose.tasks/imessagehandler) - message handler callback which can be used to intercept log messages produced by Aspose.
### getMessageLevel() {#getMessageLevel--}
```
public final int getMessageLevel()
```


リソースレベリング中に Aspose.Tasks が出力するログメッセージのレベルを取得します。

**Returns:**
int - Aspose が出力するログメッセージのレベル。
### getResources() {#getResources--}
```
public final List<Resource> getResources()
```


レベル付けされるリソースの一覧を取得します。null が設定された場合、すべてのプロジェクトリソースがレベル付けされます。

**Returns:**
java.util.List&lt;com.aspose.tasks.Resource&gt; - レベル付けされるリソースの一覧。
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


レベリング期間の開始日を取得します。デフォルト値はプロジェクトの開始日です。

**Returns:**
java.util.Date - レベリング期間の開始日。
### setCancellationToken(CancellationToken value) {#setCancellationToken-com.aspose.tasks.CancellationToken-}
```
public final void setCancellationToken(CancellationToken value)
```


プロジェクトのレベリング操作をキャンセルするために使用できるトークンを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [CancellationToken](../../com.aspose.tasks/cancellationtoken) | プロジェクトのレベリング操作をキャンセルするために使用できるトークン。 |

### setFinishDate(Date value) {#setFinishDate-java.util.Date-}
```
public final void setFinishDate(Date value)
```


レベリング期間の終了日を設定します。デフォルト値はプロジェクトの完了日です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | レベリング期間の終了日。 |

### setLevelingOrder(int value) {#setLevelingOrder-int-}
```
public final void setLevelingOrder(int value)
```


レベリングアルゴリズムが過剰割り当てのあるタスクを遅延させる順序です。過剰割り当てを引き起こすタスクと遅延可能なタスクを特定した後、どのタスクを最初に遅延させるかを指定された順序で使用します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | レベリングアルゴリズムが過剰割り当てのあるタスクを遅延させる順序。 |

### setMessageHandler(IMessageHandler value) {#setMessageHandler-com.aspose.tasks.IMessageHandler-}
```
public final void setMessageHandler(IMessageHandler value)
```


リソースレベリング中に Aspose.Tasks が生成するログメッセージをインターセプトできるメッセージハンドラコールバックを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [IMessageHandler](../../com.aspose.tasks/imessagehandler) | Aspose が生成するログメッセージをインターセプトできるメッセージハンドラコールバック。 |

### setMessageLevel(int value) {#setMessageLevel-int-}
```
public final void setMessageLevel(int value)
```


リソースレベリング中に Aspose.Tasks が出力するログメッセージのレベルを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | Aspose が出力するログメッセージのレベル。 |

### setResources(List&lt;Resource&gt; value) {#setResources-java.util.List-com.aspose.tasks.Resource--}
```
public final void setResources(List<Resource> value)
```


レベル付けされるリソースの一覧を設定します。null が設定された場合、すべてのプロジェクトリソースがレベル付けされます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.List&lt;com.aspose.tasks.Resource&gt; | レベル付けされるリソースの一覧。 |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


レベリング期間の開始日を設定します。デフォルト値はプロジェクトの開始日です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | レベリング期間の開始日。 |

