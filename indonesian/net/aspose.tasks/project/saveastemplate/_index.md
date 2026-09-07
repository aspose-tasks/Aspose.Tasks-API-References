---
title: "Project.SaveAsTemplate"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Project. Menyimpan proyek sebagai templat."
type: docs
weight: 1210
url: /id/net/aspose.tasks/project/saveastemplate/
---
## SaveAsTemplate(string, SaveTemplateOptions) {#saveastemplate_3}

Menyimpan proyek sebagai templat.

```csharp
public void SaveAsTemplate(string fileName, SaveTemplateOptions options)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileName | String | Nama file. |
| options | SaveTemplateOptions | opsi penyimpanan yang ditentukan [`SaveTemplateOptions`](../../../aspose.tasks.saving/savetemplateoptions/). |

## Contoh

Menampilkan cara menyimpan proyek sebagai templat.

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

### Lihat Juga

* class [SaveTemplateOptions](../../../aspose.tasks.saving/savetemplateoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveAsTemplate(string) {#saveastemplate_2}

Menyimpan proyek sebagai templat ke jalur file yang ditentukan.

```csharp
public void SaveAsTemplate(string fileName)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileName | String | nama file yang ditentukan. |

## Contoh

Menampilkan cara menyimpan proyek sebagai templat.

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

### Lihat Juga

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveAsTemplate(Stream) {#saveastemplate}

Menyimpan proyek sebagai templat ke aliran yang ditentukan.

```csharp
public void SaveAsTemplate(Stream stream)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | Stream | aliran yang ditentukan untuk menyimpan proyek. |

## Contoh

Menampilkan cara menyimpan proyek sebagai templat.

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

### Lihat Juga

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveAsTemplate(Stream, SaveTemplateOptions) {#saveastemplate_1}

Menyimpan proyek sebagai templat ke aliran yang ditentukan.

```csharp
public void SaveAsTemplate(Stream stream, SaveTemplateOptions options)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | Stream | Aliran untuk menyimpan templat proyek. |
| options | SaveTemplateOptions | opsi penyimpanan yang ditentukan [`SaveTemplateOptions`](../../../aspose.tasks.saving/savetemplateoptions/). |

## Contoh

Menampilkan cara menyimpan proyek sebagai templat.

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

### Lihat Juga

* class [SaveTemplateOptions](../../../aspose.tasks.saving/savetemplateoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


