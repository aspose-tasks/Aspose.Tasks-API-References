---
title: PrimaveraXmlReader.PrimaveraXmlReader
second_title: Aspose.Tasks for .NET API Reference
description: PrimaveraXmlReader constructor. Initializes a new instance of the PrimaveraXmlReader class
type: docs
weight: 10
url: /net/aspose.tasks/primaveraxmlreader/primaveraxmlreader/
---
## PrimaveraXmlReader(string) {#constructor_1}

Initializes a new instance of the [`PrimaveraXmlReader`](../) class.

```csharp
public PrimaveraXmlReader(string templatePath)
```

| Parameter | Type | Description |
| --- | --- | --- |
| templatePath | String | Path to template where Primavera Xml project or projects are located |

## Examples

Shows how to examine short projects' info from a Primavera XML file.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "MultiprojectWithExternal.xml");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}
```

### See Also

* class [PrimaveraXmlReader](../)
* namespace [Aspose.Tasks](../../primaveraxmlreader/)
* assembly [Aspose.Tasks](../../../)

---

## PrimaveraXmlReader(Stream) {#constructor}

Initializes a new instance of the [`PrimaveraXmlReader`](../) class.

```csharp
public PrimaveraXmlReader(Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | Stream containing Primavera Xml content. |

## Examples

Shows how to import a project from a Primavera XML stream.

```csharp
using (var stream = new FileStream(DataDir + "primavera.xml", FileMode.Open))
{
    var reader = new PrimaveraXmlReader(stream);
    List<int> projectUids = reader.GetProjectUids();
    foreach (var projectUid in projectUids)
    {
        Console.WriteLine("Project UID: " + projectUid);
    }
}
```

### See Also

* class [PrimaveraXmlReader](../)
* namespace [Aspose.Tasks](../../primaveraxmlreader/)
* assembly [Aspose.Tasks](../../../)


