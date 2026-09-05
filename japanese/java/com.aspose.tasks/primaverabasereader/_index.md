---
title: "PrimaveraBaseReader"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "複数プロジェクトの Primavera XER または XML ファイルからプロジェクト UID を読み取るために使用できる基本リーダーを表します。"
type: docs
weight: 196
url: /ja/java/com.aspose.tasks/primaverabasereader/
---

**Inheritance:**
java.lang.Object
```
public abstract class PrimaveraBaseReader
```

複数プロジェクトの Primavera XER または XML ファイルからプロジェクト UID を読み取るために使用できる基本リーダーを表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getProjectInfos()](#getProjectInfos--) | プロジェクトの短い情報オブジェクトのリストを返します。 |
| [getProjectUids()](#getProjectUids--) | プロジェクトの一意の識別子のリストを返します。 |
| [loadProject(int projectUid)](#loadProject-int-) | 指定された一意の識別子でプロジェクトをロードします。 |
### getProjectInfos() {#getProjectInfos--}
```
public final List<PrimaveraProjectInfo> getProjectInfos()
```


プロジェクトの短い情報オブジェクトのリストを返します。

**Returns:**
java.util.List&lt;com.aspose.tasks.PrimaveraProjectInfo&gt; - プロジェクトの短い情報オブジェクトのリスト
### getProjectUids() {#getProjectUids--}
```
public final List<Integer> getProjectUids()
```


プロジェクトの一意の識別子のリストを返します。

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - プロジェクトの一意の識別子のリスト。
### loadProject(int projectUid) {#loadProject-int-}
```
public Project loadProject(int projectUid)
```


指定された一意の識別子でプロジェクトをロードします。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| projectUid | int | ロードするプロジェクトの一意の識別子です。 |

**Returns:**
[Project](../../com.aspose.tasks/project) - Project with specified unique identifier from the specified multi project file. Null if project doesn't exist.
