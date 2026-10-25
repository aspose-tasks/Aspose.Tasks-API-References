---
title: "Project.SaveAsTemplate"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método del proyecto. Guarda el proyecto como una plantilla."
type: docs
weight: 1210
url: /es/net/aspose.tasks/project/saveastemplate/
---
## SaveAsTemplate(string, SaveTemplateOptions) {#saveastemplate_3}

Guarda el proyecto como una plantilla.

```csharp
public void SaveAsTemplate(string fileName, SaveTemplateOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | Cadena | El nombre del archivo. |
| options | SaveTemplateOptions | las opciones de guardado especificadas [`SaveTemplateOptions`](../../../aspose.tasks.saving/savetemplateoptions/). |

## Ejemplos

Muestra cómo guardar el proyecto como una plantilla.

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

### Ver también

* class [SaveTemplateOptions](../../../aspose.tasks.saving/savetemplateoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveAsTemplate(string) {#saveastemplate_2}

Guarda el proyecto como una plantilla en la ruta de archivo especificada.

```csharp
public void SaveAsTemplate(string fileName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | Cadena | el nombre de archivo especificado. |

## Ejemplos

Muestra cómo guardar el proyecto como una plantilla.

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

### Ver también

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveAsTemplate(Stream) {#saveastemplate}

Guarda el proyecto como una plantilla en un flujo especificado.

```csharp
public void SaveAsTemplate(Stream stream)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | Flujo | el flujo especificado para guardar el proyecto. |

## Ejemplos

Muestra cómo guardar el proyecto como una plantilla.

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

### Ver también

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveAsTemplate(Stream, SaveTemplateOptions) {#saveastemplate_1}

Guarda el proyecto como una plantilla en un flujo especificado.

```csharp
public void SaveAsTemplate(Stream stream, SaveTemplateOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | Flujo | Flujo para guardar la plantilla del proyecto. |
| options | SaveTemplateOptions | las opciones de guardado especificadas [`SaveTemplateOptions`](../../../aspose.tasks.saving/savetemplateoptions/). |

## Ejemplos

Muestra cómo guardar el proyecto como una plantilla.

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

### Ver también

* class [SaveTemplateOptions](../../../aspose.tasks.saving/savetemplateoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


