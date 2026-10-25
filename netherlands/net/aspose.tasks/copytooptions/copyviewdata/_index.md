---
title: "CopyToOptions.CopyViewData"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "CopyToOptions-eigenschap. Haalt een waarde op of stelt deze in die aangeeft of weergavegegevens moeten worden gekopieerd tijdens het kopiëren van projectgegevens. Standaardwaarde is true"
type: docs
weight: 20
url: /nl/net/aspose.tasks/copytooptions/copyviewdata/
---
## CopyToOptions.CopyViewData property

Haalt of stelt een waarde in die aangeeft of weergavegegevens moeten worden gekopieerd tijdens het kopiëren van projectgegevens. Standaardwaarde is true.

```csharp
public bool CopyViewData { get; set; }
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


