---
title: "ProjectServerSaveOptions"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "プロジェクトを Project Server または Project Online に保存する際に、追加オプションを指定できます。"
type: docs
weight: 227
url: /ja/java/com.aspose.tasks/projectserversaveoptions/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerSaveOptions
```

プロジェクトを Project Server または Project Online に保存する際に、追加オプションを指定できます。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [ProjectServerSaveOptions()](#ProjectServerSaveOptions--) | 新しい [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getPollingInterval()](#getPollingInterval--) | キュー ジョブ ステータス要求間の間隔を取得します。 |
| [getProjectGuid()](#getProjectGuid--) | プロジェクトの一意の識別子を取得します。 |
| [getProjectName()](#getProjectName--) | Project Server \\ Project Online のプロジェクト一覧に表示されるプロジェクト名を取得します。 |
| [getTimeout()](#getTimeout--) | Project Server のキュー処理サービスがプロジェクト保存要求の処理を待機する際に使用されるタイムアウトを取得します。 |
| [setPollingInterval(double value)](#setPollingInterval-double-) | キュー ジョブ ステータス要求間の間隔を設定します。 |
| [setProjectGuid(UUID value)](#setProjectGuid-java.util.UUID-) | プロジェクトの一意の識別子を設定します。 |
| [setProjectName(String value)](#setProjectName-java.lang.String-) | Project Server \\ Project Online のプロジェクト一覧に表示されるプロジェクト名を設定します。 |
| [setTimeout(double value)](#setTimeout-double-) | Project Server のキュー処理サービスがプロジェクト保存要求の処理を待機する際に使用されるタイムアウトを設定します。 |
### ProjectServerSaveOptions() {#ProjectServerSaveOptions--}
```
public ProjectServerSaveOptions()
```


新しい [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) クラスのインスタンスを初期化します。

### getPollingInterval() {#getPollingInterval--}
```
public final double getPollingInterval()
```


キュー ジョブ ステータス要求間の間隔を取得します。デフォルト値は 2 秒です。

**Returns:**
double - キュー ジョブ ステータス要求間の間隔。
### getProjectGuid() {#getProjectGuid--}
```
public final UUID getProjectGuid()
```


プロジェクトの一意の識別子を取得します。Project Server \\ Project Online インスタンス内で一意である必要があります。

**Returns:**
java.util.UUID - プロジェクトの一意の識別子。
### getProjectName() {#getProjectName--}
```
public final String getProjectName()
```


Project Server \\ Project Online のプロジェクト一覧に表示されるプロジェクト名を取得します。Project Server \\ Project Online インスタンス内で一意である必要があります。値が省略された場合、代わりに Prj.Name プロパティの値が使用されます。

**Returns:**
java.lang.String - Project Server \\ Project Online のプロジェクト一覧に表示されるプロジェクト名。
### getTimeout() {#getTimeout--}
```
public final double getTimeout()
```


Project Server のキュー処理サービスがプロジェクト保存要求の処理を待機する際に使用されるタイムアウトを取得します。このプロパティのデフォルト値は 1 分です。

--------------------

大規模なプロジェクトや、Project Server インスタンスが他の要求への応答で過度に忙しい場合、処理時間が長くなることがあります。

**Returns:**
double - Project Server のキュー処理サービスがプロジェクト保存要求の処理を待機する際に使用されるタイムアウト。
### setPollingInterval(double value) {#setPollingInterval-double-}
```
public final void setPollingInterval(double value)
```


キュー ジョブ ステータス要求間の間隔を設定します。デフォルト値は 2 秒です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | キュー ジョブ ステータス要求間の間隔。 |

### setProjectGuid(UUID value) {#setProjectGuid-java.util.UUID-}
```
public final void setProjectGuid(UUID value)
```


プロジェクトの一意の識別子を設定します。Project Server \\ Project Online インスタンス内で一意である必要があります。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.UUID | プロジェクトの一意の識別子。 |

### setProjectName(String value) {#setProjectName-java.lang.String-}
```
public final void setProjectName(String value)
```


Project Server \\ Project Online のプロジェクト一覧に表示されるプロジェクト名を設定します。Project Server \\ Project Online インスタンス内で一意である必要があります。値が省略された場合、代わりに Prj.Name プロパティの値が使用されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | Project Server \\ Project Online のプロジェクト一覧に表示されるプロジェクト名。 |

### setTimeout(double value) {#setTimeout-double-}
```
public final void setTimeout(double value)
```


Project Server のキュー処理サービスがプロジェクト保存要求の処理を待機する際に使用されるタイムアウトを設定します。このプロパティのデフォルト値は 1 分です。

--------------------

大規模なプロジェクトや、Project Server インスタンスが他の要求への応答で過度に忙しい場合、処理時間が長くなることがあります。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | Project Server のキュー処理サービスによるプロジェクト保存リクエストの処理を待機中に使用されるタイムアウト。 |

