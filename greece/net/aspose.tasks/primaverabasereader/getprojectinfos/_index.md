---
title: "PrimaveraBaseReader.GetProjectInfos"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος PrimaveraBaseReader. Επιστρέφει μια λίστα με τα αντικείμενα σύντομης πληροφορίας των έργων"
type: docs
weight: 10
url: /el/net/aspose.tasks/primaverabasereader/getprojectinfos/
---
## PrimaveraBaseReader.GetProjectInfos method

Επιστρέφει μια λίστα με τα σύντομα αντικείμενα πληροφοριών του έργου.

```csharp
public List<PrimaveraProjectInfo> GetProjectInfos()
```

## Παραδείγματα

Δείχνει πώς να εξετάσετε τις πληροφορίες σύντομων έργων από ένα αρχείο Primavera XML.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "MultiprojectWithExternal.xml");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}
```

Δείχνει πώς να εξετάσετε τις πληροφορίες σύντομων έργων από ένα αρχείο Primavera XER.

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

Δείχνει πώς να λάβετε σύντομες πληροφορίες των έργων από μια βάση δεδομένων Primavera.

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

### Δείτε επίσης

* class [PrimaveraProjectInfo](../../../aspose.tasks.primavera/primaveraprojectinfo/)
* class [PrimaveraBaseReader](../)
* namespace [Aspose.Tasks](../../primaverabasereader/)
* assembly [Aspose.Tasks](../../../)


