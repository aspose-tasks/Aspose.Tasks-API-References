---
title: "PrimaveraBaseReader.GetProjectInfos"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "PrimaveraBaseReader メソッド。プロジェクトの短い情報オブジェクトのリストを返します"
type: docs
weight: 10
url: /ja/net/aspose.tasks/primaverabasereader/getprojectinfos/
---
## PrimaveraBaseReader.GetProjectInfos method

プロジェクトの簡易情報オブジェクトのリストを返します。

```csharp
public List<PrimaveraProjectInfo> GetProjectInfos()
```

## 例

Primavera XML ファイルからプロジェクトの短い情報を調べる方法を示します。

```csharp
var reader = new PrimaveraXmlReader(DataDir + "MultiprojectWithExternal.xml");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}
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

Primavera データベースからプロジェクトの簡易情報を取得する方法を示します。

```csharp
var settings = new PrimaveraDbSettings(GetConnectionString(), 0);

var reader = new PrimaveraDbReader(settings);
var projectInfos = reader.GetProjectInfos();

foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - '{2}'", info.Uid, info.ShortName, info.Name);
}

var firstProject = reader.LoadProject(projectInfos[0].Uid);
Console.WriteLine(firstProject.Uid);
Console.WriteLine(firstProject.Name);
Console.WriteLine(firstProject.PrimaveraProperties.ShortName);
```

### 関連項目

* class [PrimaveraProjectInfo](../../../aspose.tasks.primavera/primaveraprojectinfo/)
* class [PrimaveraBaseReader](../)
* namespace [Aspose.Tasks](../../primaverabasereader/)
* assembly [Aspose.Tasks](../../../)


