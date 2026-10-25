---
title: "PrimaveraBaseReader.LoadProject"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PrimaveraBaseReader yöntemi. Belirtilen benzersiz tanımlayıcıya sahip projeyi yükler"
type: docs
weight: 30
url: /tr/net/aspose.tasks/primaverabasereader/loadproject/
---
## PrimaveraBaseReader.LoadProject method

Belirtilen benzersiz tanımlayıcıya sahip projeyi yükler.

```csharp
public virtual Project LoadProject(int projectUid)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| projectUid | Int32 | Yüklenecek projenin benzersiz tanımlayıcısı. |

### Dönüş Değeri

Belirtilen çoklu proje dosyasından belirtilen benzersiz tanımlayıcıya sahip proje. Proje mevcut değilse Null.

## Örnekler

Projeyi uid'si bilindiğinde bir Primavera XML dosyasından nasıl yükleyeceğini gösterir.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "PrimaveraProject.xml");
var project = reader.LoadProject(3882);
Console.WriteLine(project.Name);
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

### Ayrıca Bakınız

* class [Project](../../project/)
* class [PrimaveraBaseReader](../)
* namespace [Aspose.Tasks](../../primaverabasereader/)
* assembly [Aspose.Tasks](../../../)


