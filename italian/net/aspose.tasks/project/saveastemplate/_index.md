---
title: "Project.SaveAsTemplate"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo di Project. Salva il progetto come modello."
type: docs
weight: 1210
url: /it/net/aspose.tasks/project/saveastemplate/
---
## SaveAsTemplate(string, SaveTemplateOptions) {#saveastemplate_3}

Salva il progetto come modello.

```csharp
public void SaveAsTemplate(string fileName, SaveTemplateOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | Stringa | Il nome del file. |
| options | SaveTemplateOptions | le opzioni di salvataggio specificate [`SaveTemplateOptions`](../../../aspose.tasks.saving/savetemplateoptions/). |

## Esempi

Mostra come salvare il progetto come modello.

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

### Vedi anche

* class [SaveTemplateOptions](../../../aspose.tasks.saving/savetemplateoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveAsTemplate(string) {#saveastemplate_2}

Salva il progetto come modello nel percorso file specificato.

```csharp
public void SaveAsTemplate(string fileName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | Stringa | il nome del file specificato. |

## Esempi

Mostra come salvare il progetto come modello.

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

### Vedi anche

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveAsTemplate(Stream) {#saveastemplate}

Salva il progetto come modello in uno stream specificato.

```csharp
public void SaveAsTemplate(Stream stream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | Flusso | lo stream specificato su cui salvare il progetto. |

## Esempi

Mostra come salvare il progetto come modello.

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

### Vedi anche

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveAsTemplate(Stream, SaveTemplateOptions) {#saveastemplate_1}

Salva il progetto come modello in uno stream specificato.

```csharp
public void SaveAsTemplate(Stream stream, SaveTemplateOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | Flusso | Stream su cui salvare il modello del progetto. |
| options | SaveTemplateOptions | le opzioni di salvataggio specificate [`SaveTemplateOptions`](../../../aspose.tasks.saving/savetemplateoptions/). |

## Esempi

Mostra come salvare il progetto come modello.

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

### Vedi anche

* class [SaveTemplateOptions](../../../aspose.tasks.saving/savetemplateoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


