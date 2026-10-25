---
title: "PrimaveraBaseReader.LoadProject"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "PrimaveraBaseReader メソッド。指定されたユニーク識別子を持つプロジェクトをロードします"
type: docs
weight: 30
url: /ja/net/aspose.tasks/primaverabasereader/loadproject/
---
## PrimaveraBaseReader.LoadProject method

指定された一意の識別子でプロジェクトをロードします。

```csharp
public virtual Project LoadProject(int projectUid)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| projectUid | Int32 | 読み込むプロジェクトの一意の識別子です。 |

### 戻り値

指定されたマルチプロジェクトファイルから、指定されたユニーク識別子を持つプロジェクト。存在しない場合は null です。

## 例

プロジェクト UID が既知の場合に、Primavera XML ファイルからプロジェクトをロードする方法を示します。

```csharp
var reader = new PrimaveraXmlReader(DataDir + "PrimaveraProject.xml");
var project = reader.LoadProject(3882);
Console.WriteLine(project.Name);
```

Primavera XER ファイルからプロジェクトの短い情報を調べる方法を示します。

```csharp
var reader = new PrimaveraXerReader(DataDir + "MultiprojectWithExternal.xer");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}

var project = reader.LoadProject(5494);

Console.WriteLine("Loaded project '{0}' with Uid {1}", project.Name, project.Uid);
```

### 関連項目

* class [Project](../../project/)
* class [PrimaveraBaseReader](../)
* namespace [Aspose.Tasks](../../primaverabasereader/)
* assembly [Aspose.Tasks](../../../)


