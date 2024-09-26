---
title: PrimaveraXerReader.PrimaveraXerReader
second_title: Aspose.Tasks for .NET API Reference
description: PrimaveraXerReader constructor. Initializes a new instance of the PrimaveraXerReader class
type: docs
weight: 10
url: /net/aspose.tasks/primaveraxerreader/primaveraxerreader/
---
## PrimaveraXerReader(string) {#constructor_1}

Initializes a new instance of the [`PrimaveraXerReader`](../) class.

```csharp
public PrimaveraXerReader(string xerFilePath)
```

| Parameter | Type | Description |
| --- | --- | --- |
| xerFilePath | String | Path to .xer file where Primavera project or projects are located. |

## Examples

Shows how to examine short projects' info from a Primavera XER file.

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

### See Also

* class [PrimaveraXerReader](../)
* namespace [Aspose.Tasks](../../primaveraxerreader/)
* assembly [Aspose.Tasks](../../../)

---

## PrimaveraXerReader(Stream) {#constructor}

Initializes a new instance of the [`PrimaveraXerReader`](../) class.

```csharp
public PrimaveraXerReader(Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | Stream with Primavera XER content. |

### See Also

* class [PrimaveraXerReader](../)
* namespace [Aspose.Tasks](../../primaveraxerreader/)
* assembly [Aspose.Tasks](../../../)


