---
title: "Project.SaveAsTemplate"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project मेथड। प्रोजेक्ट को एक टेम्पलेट के रूप में सहेजता है।"
type: docs
weight: 1210
url: /hi/net/aspose.tasks/project/saveastemplate/
---
## SaveAsTemplate(string, SaveTemplateOptions) {#saveastemplate_3}

परियोजना को टेम्प्लेट के रूप में सहेजता है।

```csharp
public void SaveAsTemplate(string fileName, SaveTemplateOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileName | स्ट्रिंग | फ़ाइल का नाम। |
| options | SaveTemplateOptions | निर्दिष्ट सहेजने के विकल्प [`SaveTemplateOptions`](../../../aspose.tasks.saving/savetemplateoptions/). |

## उदाहरण

दिखाता है कि कैसे प्रोजेक्ट को टेम्पलेट के रूप में सहेजा जाए।

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

### संबंधित देखें

* class [SaveTemplateOptions](../../../aspose.tasks.saving/savetemplateoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveAsTemplate(string) {#saveastemplate_2}

परियोजना को टेम्प्लेट के रूप में निर्दिष्ट फ़ाइल पथ में सहेजता है।

```csharp
public void SaveAsTemplate(string fileName)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileName | स्ट्रिंग | निर्दिष्ट फ़ाइल नाम। |

## उदाहरण

दिखाता है कि कैसे प्रोजेक्ट को टेम्पलेट के रूप में सहेजा जाए।

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

### संबंधित देखें

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveAsTemplate(Stream) {#saveastemplate}

परियोजना को टेम्प्लेट के रूप में निर्दिष्ट स्ट्रीम में सहेजता है।

```csharp
public void SaveAsTemplate(Stream stream)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| स्ट्रीम | स्ट्रीम | निर्दिष्ट स्ट्रीम जहाँ प्रोजेक्ट को सहेजा जाना है। |

## उदाहरण

दिखाता है कि कैसे प्रोजेक्ट को टेम्पलेट के रूप में सहेजा जाए।

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

### संबंधित देखें

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveAsTemplate(Stream, SaveTemplateOptions) {#saveastemplate_1}

परियोजना को टेम्प्लेट के रूप में निर्दिष्ट स्ट्रीम में सहेजता है।

```csharp
public void SaveAsTemplate(Stream stream, SaveTemplateOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| स्ट्रीम | स्ट्रीम | स्ट्रीम जहाँ प्रोजेक्ट टेम्पलेट को सहेजा जाएगा। |
| options | SaveTemplateOptions | निर्दिष्ट सहेजने के विकल्प [`SaveTemplateOptions`](../../../aspose.tasks.saving/savetemplateoptions/). |

## उदाहरण

दिखाता है कि कैसे प्रोजेक्ट को टेम्पलेट के रूप में सहेजा जाए।

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

### संबंधित देखें

* class [SaveTemplateOptions](../../../aspose.tasks.saving/savetemplateoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


