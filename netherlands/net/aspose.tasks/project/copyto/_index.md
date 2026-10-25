---
title: "Project.CopyTo"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Project methode. Kopieert de hoofdgegevens en -eigenschappen van het project naar een ander project."
type: docs
weight: 1060
url: /nl/net/aspose.tasks/project/copyto/
---
## CopyTo(Project) {#copyto}

Kopieert de hoofdgegevens en eigenschappen van het project naar een ander project.

```csharp
public void CopyTo(Project another)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| ander | Project | Een ander project om gegevens naartoe te kopiëren. |

## Voorbeelden

Toont hoe de projectgegevens naar een ander project te kopiëren.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", DataDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(DataDir + "ProjectCopying_out.mpp");

// sla kopiëren van weergavegegevens over tijdens het kopiëren van algemene projectgegevens.
project.CopyTo(mppProject);
```

### Zie ook

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## CopyTo(Project, CopyToOptions) {#copyto_1}

Kopieert de hoofdgegevens en eigenschappen van het project naar een ander project.

```csharp
public void CopyTo(Project another, CopyToOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| ander | Project | Een ander project om gegevens naartoe te kopiëren. |
| opties | CopyToOptions | Kopieeropties om het kopieerproces te beheersen. |

## Voorbeelden

Toont hoe het project te kopiëren met gebruik van &lt;see cref=\"Aspose.Tasks.CopyToOptions\"/&gt; instantie.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", OutDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(OutDir + "ProjectCopying_out.mpp");

// sla kopiëren van weergavegegevens over tijdens het kopiëren van algemene projectgegevens.
var options = new CopyToOptions
{
    CopyViewData = false
};
project.CopyTo(mppProject, options);
```

### Zie ook

* class [CopyToOptions](../../copytooptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


