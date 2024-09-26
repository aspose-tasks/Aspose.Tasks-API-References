---
title: Project.SaveAsTemplate
second_title: Aspose.Tasks for .NET API Reference
description: Project method. Saves the project as a template
type: docs
weight: 1210
url: /net/aspose.tasks/project/saveastemplate/
---
## SaveAsTemplate(string, SaveTemplateOptions) {#saveastemplate_3}

Saves the project as a template.

```csharp
public void SaveAsTemplate(string fileName, SaveTemplateOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The file name. |
| options | SaveTemplateOptions | the specified save options [`SaveTemplateOptions`](../../../aspose.tasks.saving/savetemplateoptions/). |

## Examples

Shows how to save project as a template.

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

### See Also

* class [SaveTemplateOptions](../../../aspose.tasks.saving/savetemplateoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveAsTemplate(string) {#saveastemplate_2}

Saves the project as a template to the specified file path.

```csharp
public void SaveAsTemplate(string fileName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | the specified file name. |

## Examples

Shows how to save project as a template.

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

### See Also

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveAsTemplate(Stream) {#saveastemplate}

Saves the project as a template to a specified stream.

```csharp
public void SaveAsTemplate(Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | the specified stream to save the project to. |

## Examples

Shows how to save project as a template.

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

### See Also

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveAsTemplate(Stream, SaveTemplateOptions) {#saveastemplate_1}

Saves the project as a template to a specified stream.

```csharp
public void SaveAsTemplate(Stream stream, SaveTemplateOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | Stream to save the project template to. |
| options | SaveTemplateOptions | the specified save options [`SaveTemplateOptions`](../../../aspose.tasks.saving/savetemplateoptions/). |

## Examples

Shows how to save project as a template.

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

### See Also

* class [SaveTemplateOptions](../../../aspose.tasks.saving/savetemplateoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


