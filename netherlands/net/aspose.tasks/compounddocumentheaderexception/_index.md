---
title: "Klasse CompoundDocumentHeaderException"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.CompoundDocumentHeaderException klasse. Vertegenwoordigt een uitzondering die wordt gegooid wanneer de header van een MPP‑bestand beschadigd is."
type: docs
weight: 280
url: /nl/net/aspose.tasks/compounddocumentheaderexception/
---
## CompoundDocumentHeaderException class

Stelt een uitzondering voor die wordt gegooid wanneer de header van een MPP‑bestand beschadigd is.

```csharp
public class CompoundDocumentHeaderException : ApplicationException
```

## Voorbeelden

Toont hoe &lt;see cref=\"CompoundDocumentHeaderException\" /&gt; uitzondering op te vangen.

```csharp
try
{
    var project = new Project(DataDir + "Project1.mpp");

    Console.WriteLine("Project Name: " + project.Get(Prj.Name));
}
catch (CompoundDocumentHeaderException e)
{
    Console.WriteLine(e.Message);
}
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


