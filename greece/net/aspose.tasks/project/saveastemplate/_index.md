---
title: "Project.SaveAsTemplate"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Project. Αποθηκεύει το έργο ως πρότυπο"
type: docs
weight: 1210
url: /el/net/aspose.tasks/project/saveastemplate/
---
## SaveAsTemplate(string, SaveTemplateOptions) {#saveastemplate_3}

Αποθηκεύει το έργο ως πρότυπο.

```csharp
public void SaveAsTemplate(string fileName, SaveTemplateOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | String | Το όνομα αρχείου. |
| options | SaveTemplateOptions | η καθορισμένη επιλογή αποθήκευσης [`SaveTemplateOptions`](../../../aspose.tasks.saving/savetemplateoptions/). |

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε το έργο ως πρότυπο.

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

### Δείτε επίσης

* class [SaveTemplateOptions](../../../aspose.tasks.saving/savetemplateoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveAsTemplate(string) {#saveastemplate_2}

Αποθηκεύει το έργο ως πρότυπο στη καθορισμένη διαδρομή αρχείου.

```csharp
public void SaveAsTemplate(string fileName)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | String | το καθορισμένο όνομα αρχείου. |

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε το έργο ως πρότυπο.

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

### Δείτε επίσης

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveAsTemplate(Stream) {#saveastemplate}

Αποθηκεύει το έργο ως πρότυπο σε μια καθορισμένη ροή.

```csharp
public void SaveAsTemplate(Stream stream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | Ροή | η καθορισμένη ροή για αποθήκευση του έργου. |

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε το έργο ως πρότυπο.

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

### Δείτε επίσης

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveAsTemplate(Stream, SaveTemplateOptions) {#saveastemplate_1}

Αποθηκεύει το έργο ως πρότυπο σε μια καθορισμένη ροή.

```csharp
public void SaveAsTemplate(Stream stream, SaveTemplateOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | Ροή | Ροή για αποθήκευση του προτύπου έργου. |
| options | SaveTemplateOptions | η καθορισμένη επιλογή αποθήκευσης [`SaveTemplateOptions`](../../../aspose.tasks.saving/savetemplateoptions/). |

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε το έργο ως πρότυπο.

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

### Δείτε επίσης

* class [SaveTemplateOptions](../../../aspose.tasks.saving/savetemplateoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


