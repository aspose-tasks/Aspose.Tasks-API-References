---
title: "ResourceLeveler"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "リソース平準化メソッドを含みます。"
type: docs
weight: 253
url: /ja/java/com.aspose.tasks/resourceleveler/
---

**Inheritance:**
java.lang.Object
```
public class ResourceLeveler
```

リソース平準化メソッドを含みます。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [ResourceLeveler()](#ResourceLeveler--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [clearLeveling(Project project)](#clearLeveling-com.aspose.tasks.Project-) | リソース レベリング中にプロジェクトに以前追加されたレベリング遅延をすべてクリアします。 |
| [clearLeveling(Iterable&lt;Task&gt; tasks)](#clearLeveling-java.lang.Iterable-com.aspose.tasks.Task--) | リソース レベリング中に指定されたタスクに以前追加されたレベリング遅延をすべてクリアします。 |
| [levelAll(Project project)](#levelAll-com.aspose.tasks.Project-) | デフォルトのレベリングオプションを使用して、プロジェクトのすべてのリソースのタスクをレベル設定します。 |
| [levelResources(Project project, LevelingOptions options)](#levelResources-com.aspose.tasks.Project-com.aspose.tasks.LevelingOptions-) | 指定されたレベリングオプションを使用して、指定されたリソースのタスクをレベル設定します。 |
### ResourceLeveler() {#ResourceLeveler--}
```
public ResourceLeveler()
```


### clearLeveling(Project project) {#clearLeveling-com.aspose.tasks.Project-}
```
public static void clearLeveling(Project project)
```


リソース レベリング中にプロジェクトに以前追加されたレベリング遅延をすべてクリアします。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | レベリングをクリアするプロジェクト。 |

### clearLeveling(Iterable&lt;Task&gt; tasks) {#clearLeveling-java.lang.Iterable-com.aspose.tasks.Task--}
```
public static void clearLeveling(Iterable<Task> tasks)
```


リソース レベリング中に指定されたタスクに以前追加されたレベリング遅延をすべてクリアします。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| タスク | java.lang.Iterable&lt;com.aspose.tasks.Task&gt; | レベリング遅延をクリアすべきタスクを含む列挙体。 |

### levelAll(Project project) {#levelAll-com.aspose.tasks.Project-}
```
public static LevelingResult levelAll(Project project)
```


デフォルトのレベリングオプションを使用して、プロジェクトのすべてのリソースのタスクをレベル設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | リソース レベリングを適用するプロジェクト。 |

**Returns:**
[LevelingResult](../../com.aspose.tasks/levelingresult) - Object containing results of resource leveling.
### levelResources(Project project, LevelingOptions options) {#levelResources-com.aspose.tasks.Project-com.aspose.tasks.LevelingOptions-}
```
public static LevelingResult levelResources(Project project, LevelingOptions options)
```


指定されたレベリングオプションを使用して、指定されたリソースのタスクをレベル設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | リソース レベリングを適用するプロジェクト。 |
| options | [LevelingOptions](../../com.aspose.tasks/levelingoptions) | リソースをレベル設定する方法を指定するオプション。 |

**Returns:**
[LevelingResult](../../com.aspose.tasks/levelingresult) - Object containing results of resource leveling.
