---
title: "Project.SaveAsTemplate"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Project‑methode. Slaat het project op als een sjabloon"
type: docs
weight: 1210
url: /nl/net/aspose.tasks/project/saveastemplate/
---
## SaveAsTemplate(string, SaveTemplateOptions) {#saveastemplate_3}

Slaat het project op als sjabloon.

```csharp
public void SaveAsTemplate(string fileName, SaveTemplateOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileName | String | De bestandsnaam. |
| options | SaveTemplateOptions | de opgegeven opslaan‑opties [`SaveTemplateOptions`](../../../aspose.tasks.saving/savetemplateoptions/). |

## Voorbeelden

Toont hoe een project op te slaan als een sjabloon.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var projectFileInfo = Project.GetProjectFileInfo(DataDir + "Project2.mpp");

if (FileFormat.MPP14 == projectFileInfo.ProjectFileFormat)
{
    Console.WriteLine("Project file format is ok");
}

var options = new SaveTemplateOptions
{
    RemoveActualValues = true,
    RemoveBaselineValues = true
};

project.SaveAsTemplate(OutDir + "SaveProjectDataAsTemplate_out.mpt", options);

var templateFileInfo = Project.GetProjectFileInfo(OutDir + "SaveProjectDataAsTemplate_out.mpt");
if (FileFormat.MPT14 == templateFileInfo.ProjectFileFormat)
{
    Console.WriteLine("Template FileFormat is ok");
}
```

### Zie ook

* class [SaveTemplateOptions](../../../aspose.tasks.saving/savetemplateoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveAsTemplate(string) {#saveastemplate_2}

Slaat het project op als sjabloon op het opgegeven bestandspad.

```csharp
public void SaveAsTemplate(string fileName)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileName | String | de opgegeven bestandsnaam. |

## Voorbeelden

Toont hoe een project op te slaan als een sjabloon.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var projectFileInfo = Project.GetProjectFileInfo(DataDir + "Project2.mpp");

if (FileFormat.MPP14 == projectFileInfo.ProjectFileFormat)
{
    Console.WriteLine("Project file format is ok");
}

var options = new SaveTemplateOptions
{
    RemoveActualValues = true,
    RemoveBaselineValues = true
};

project.SaveAsTemplate(OutDir + "SaveProjectDataAsTemplate_out.mpt", options);

var templateFileInfo = Project.GetProjectFileInfo(OutDir + "SaveProjectDataAsTemplate_out.mpt");
if (FileFormat.MPT14 == templateFileInfo.ProjectFileFormat)
{
    Console.WriteLine("Template FileFormat is ok");
}
```

### Zie ook

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveAsTemplate(Stream) {#saveastemplate}

Slaat het project op als sjabloon in een opgegeven stream.

```csharp
public void SaveAsTemplate(Stream stream)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stroom | Stroom | de opgegeven stream om het project in op te slaan. |

## Voorbeelden

Toont hoe een project op te slaan als een sjabloon.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var projectFileInfo = Project.GetProjectFileInfo(DataDir + "Project2.mpp");

if (FileFormat.MPP14 == projectFileInfo.ProjectFileFormat)
{
    Console.WriteLine("Project file format is ok");
}

var options = new SaveTemplateOptions
{
    RemoveActualValues = true,
    RemoveBaselineValues = true
};

project.SaveAsTemplate(OutDir + "SaveProjectDataAsTemplate_out.mpt", options);

var templateFileInfo = Project.GetProjectFileInfo(OutDir + "SaveProjectDataAsTemplate_out.mpt");
if (FileFormat.MPT14 == templateFileInfo.ProjectFileFormat)
{
    Console.WriteLine("Template FileFormat is ok");
}
```

### Zie ook

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveAsTemplate(Stream, SaveTemplateOptions) {#saveastemplate_1}

Slaat het project op als sjabloon in een opgegeven stream.

```csharp
public void SaveAsTemplate(Stream stream, SaveTemplateOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stroom | Stroom | Stream om het projectsjabloon in op te slaan. |
| options | SaveTemplateOptions | de opgegeven opslaan‑opties [`SaveTemplateOptions`](../../../aspose.tasks.saving/savetemplateoptions/). |

## Voorbeelden

Toont hoe een project op te slaan als een sjabloon.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var projectFileInfo = Project.GetProjectFileInfo(DataDir + "Project2.mpp");

if (FileFormat.MPP14 == projectFileInfo.ProjectFileFormat)
{
    Console.WriteLine("Project file format is ok");
}

var options = new SaveTemplateOptions
{
    RemoveActualValues = true,
    RemoveBaselineValues = true
};

project.SaveAsTemplate(OutDir + "SaveProjectDataAsTemplate_out.mpt", options);

var templateFileInfo = Project.GetProjectFileInfo(OutDir + "SaveProjectDataAsTemplate_out.mpt");
if (FileFormat.MPT14 == templateFileInfo.ProjectFileFormat)
{
    Console.WriteLine("Template FileFormat is ok");
}
```

### Zie ook

* class [SaveTemplateOptions](../../../aspose.tasks.saving/savetemplateoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


