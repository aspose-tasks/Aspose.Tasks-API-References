---
title: "Project.SaveAsTemplate"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode du projet. Enregistre le projet en tant que modèle"
type: docs
weight: 1210
url: /fr/net/aspose.tasks/project/saveastemplate/
---
## SaveAsTemplate(string, SaveTemplateOptions) {#saveastemplate_3}

Enregistre le projet en tant que modèle.

```csharp
public void SaveAsTemplate(string fileName, SaveTemplateOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | Chaîne | Le nom du fichier. |
| options | SaveTemplateOptions | les options d'enregistrement spécifiées [`SaveTemplateOptions`](../../../aspose.tasks.saving/savetemplateoptions/). |

## Exemples

Montre comment enregistrer le projet en tant que modèle.

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

### Voir aussi

* class [SaveTemplateOptions](../../../aspose.tasks.saving/savetemplateoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveAsTemplate(string) {#saveastemplate_2}

Enregistre le projet en tant que modèle dans le chemin de fichier spécifié.

```csharp
public void SaveAsTemplate(string fileName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | Chaîne | le nom de fichier spécifié. |

## Exemples

Montre comment enregistrer le projet en tant que modèle.

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

### Voir aussi

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveAsTemplate(Stream) {#saveastemplate}

Enregistre le projet en tant que modèle dans un flux spécifié.

```csharp
public void SaveAsTemplate(Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| flux | Flux | le flux spécifié pour enregistrer le projet. |

## Exemples

Montre comment enregistrer le projet en tant que modèle.

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

### Voir aussi

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveAsTemplate(Stream, SaveTemplateOptions) {#saveastemplate_1}

Enregistre le projet en tant que modèle dans un flux spécifié.

```csharp
public void SaveAsTemplate(Stream stream, SaveTemplateOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| flux | Flux | Flux pour enregistrer le modèle du projet. |
| options | SaveTemplateOptions | les options d'enregistrement spécifiées [`SaveTemplateOptions`](../../../aspose.tasks.saving/savetemplateoptions/). |

## Exemples

Montre comment enregistrer le projet en tant que modèle.

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

### Voir aussi

* class [SaveTemplateOptions](../../../aspose.tasks.saving/savetemplateoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


