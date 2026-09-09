---
title: "PrimaveraBaseReader.GetProjectInfos"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PrimaveraBaseReader yöntemi. Projelerin kısa bilgi nesnelerinin bir listesini döndürür"
type: docs
weight: 10
url: /tr/net/aspose.tasks/primaverabasereader/getprojectinfos/
---
## PrimaveraBaseReader.GetProjectInfos method

Projenin kısa bilgi nesnelerinin bir listesini döndür.

```csharp
public List<PrimaveraProjectInfo> GetProjectInfos()
```

## Örnekler

Bir Primavera XML dosyasından kısa projelerin bilgilerini nasıl inceleyeceğinizi gösterir.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "MultiprojectWithExternal.xml");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}
```

Bir Primavera XER dosyasından kısa projelerin bilgilerini nasıl inceleyeceğinizi gösterir.

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

Primavera veritabanından projelerin kısa bilgilerini nasıl alacağınızı gösterir.

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

### Ayrıca Bakınız

* class [PrimaveraProjectInfo](../../../aspose.tasks.primavera/primaveraprojectinfo/)
* class [PrimaveraBaseReader](../)
* namespace [Aspose.Tasks](../../primaverabasereader/)
* assembly [Aspose.Tasks](../../../)


