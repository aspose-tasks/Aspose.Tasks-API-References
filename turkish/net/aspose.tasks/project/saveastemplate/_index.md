---
title: "Project.SaveAsTemplate"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project yöntemi. Projeyi bir şablon olarak kaydeder"
type: docs
weight: 1210
url: /tr/net/aspose.tasks/project/saveastemplate/
---
## SaveAsTemplate(string, SaveTemplateOptions) {#saveastemplate_3}

Projeyi şablon olarak kaydeder.

```csharp
public void SaveAsTemplate(string fileName, SaveTemplateOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | Dize | Dosya adı. |
| options | SaveTemplateOptions | Belirtilen kaydetme seçenekleri [`SaveTemplateOptions`](../../../aspose.tasks.saving/savetemplateoptions/). |

## Örnekler

Projeyi bir şablon olarak nasıl kaydedeceğinizi gösterir.

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

### Ayrıca Bakınız

* class [SaveTemplateOptions](../../../aspose.tasks.saving/savetemplateoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveAsTemplate(string) {#saveastemplate_2}

Projeyi şablon olarak belirtilen dosya yoluna kaydeder.

```csharp
public void SaveAsTemplate(string fileName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | Dize | Belirtilen dosya adı. |

## Örnekler

Projeyi bir şablon olarak nasıl kaydedeceğinizi gösterir.

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

### Ayrıca Bakınız

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveAsTemplate(Stream) {#saveastemplate}

Projeyi şablon olarak belirtilen akışa kaydeder.

```csharp
public void SaveAsTemplate(Stream stream)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Akış | Projeyi kaydetmek için belirtilen akış. |

## Örnekler

Projeyi bir şablon olarak nasıl kaydedeceğinizi gösterir.

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

### Ayrıca Bakınız

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveAsTemplate(Stream, SaveTemplateOptions) {#saveastemplate_1}

Projeyi şablon olarak belirtilen akışa kaydeder.

```csharp
public void SaveAsTemplate(Stream stream, SaveTemplateOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Akış | Proje şablonunu kaydetmek için akış. |
| options | SaveTemplateOptions | Belirtilen kaydetme seçenekleri [`SaveTemplateOptions`](../../../aspose.tasks.saving/savetemplateoptions/). |

## Örnekler

Projeyi bir şablon olarak nasıl kaydedeceğinizi gösterir.

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

### Ayrıca Bakınız

* class [SaveTemplateOptions](../../../aspose.tasks.saving/savetemplateoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


