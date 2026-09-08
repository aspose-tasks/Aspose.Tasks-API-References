---
title: "CopyToOptions.CopyToOptions"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "CopyToOptions constructor. Initialiseert een nieuw exemplaar van de CopyToOptions klasse"
type: docs
weight: 10
url: /nl/net/aspose.tasks/copytooptions/copytooptions/
---
## CopyToOptions constructor

Initialiseert een nieuw exemplaar van de [`CopyToOptions`](../) klasse.

```csharp
public CopyToOptions()
```

## Voorbeelden

Toont hoe projectkopieeropties te gebruiken.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", OutDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(OutDir + "ProjectCopying_out.mpp");

// sla kopiëren van weergavegegevens over tijdens het kopiëren van algemene projectgegevens.
var copyToOptions = new CopyToOptions();
copyToOptions.CopyViewData = false;
project.CopyTo(mppProject, copyToOptions);
```

### Zie ook

* class [CopyToOptions](../)
* namespace [Aspose.Tasks](../../copytooptions/)
* assembly [Aspose.Tasks](../../../)


