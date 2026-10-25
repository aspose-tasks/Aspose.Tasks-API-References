---
title: "Project.SaveReport"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project मेथड। प्रोजेक्ट ओवरव्यू रिपोर्ट को स्ट्रीम में सहेजता है।"
type: docs
weight: 1220
url: /hi/net/aspose.tasks/project/savereport/
---
## SaveReport(Stream) {#savereport}

परियोजना अवलोकन रिपोर्ट को स्ट्रीम में सहेजता है।

```csharp
public void SaveReport(Stream stream)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| स्ट्रीम | स्ट्रीम | प्रोजेक्ट रिपोर्ट को सहेजने के लिए स्ट्रीम। |

## उदाहरण

दिखाता है कि प्रोजेक्ट ओवरव्यू रिपोर्ट को PDF फ़ाइल में कैसे सहेजा जाए।

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// निर्दिष्ट स्ट्रीम में ओवरव्यू रिपोर्ट को PDF फ़ाइल में सहेजें।
using (var stream = new FileStream(OutDir + "SaveProjectOverviewReport_out.pdf", FileMode.Create))
{
    project.SaveReport(stream);
}
```

### संबंधित देखें

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(string) {#savereport_2}

परियोजना अवलोकन रिपोर्ट को PDF फ़ाइल में सहेजता है।

```csharp
public void SaveReport(string fileName)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileName | स्ट्रिंग | फ़ाइल का नाम। |

## उदाहरण

दिखाता है कि प्रोजेक्ट ओवरव्यू रिपोर्ट को PDF फ़ाइल में स्ट्रीम में कैसे सहेजा जाए।

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// निर्दिष्ट पथ पर ओवरव्यू रिपोर्ट को PDF फ़ाइल में सहेजा जा सकता है।
project.SaveReport(OutDir + "SaveProjectOverviewReport_out.pdf");
```

### संबंधित देखें

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(Stream, ReportType) {#savereport_1}

निर्दिष्ट प्रकार की परियोजना रिपोर्ट को निर्दिष्ट स्ट्रीम में सहेजता है।

```csharp
public void SaveReport(Stream stream, ReportType reportType)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| स्ट्रीम | स्ट्रीम | प्रोजेक्ट रिपोर्ट को सहेजने के लिए निर्दिष्ट स्ट्रीम। |
| reportType | ReportType | निर्दिष्ट रिपोर्ट प्रकार।[`ReportType`](../../../aspose.tasks.visualization/reporttype/) |

## उदाहरण

दिखाता है कि विशिष्ट रिपोर्ट प्रकार के लिए प्रोजेक्ट रिपोर्ट को PDF फ़ाइल में कैसे सहेजा जाए।

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// निर्दिष्ट स्ट्रीम में ओवरव्यू रिपोर्ट को PDF फ़ाइल में सहेजें।
using (var stream = new FileStream(OutDir + "SaveProjectOverviewReport_out.pdf", FileMode.Create))
{
    project.SaveReport(stream, ReportType.Burndown);
}
```

### संबंधित देखें

* enum [ReportType](../../../aspose.tasks.visualization/reporttype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(string, ReportType) {#savereport_3}

निर्दिष्ट प्रकार की परियोजना रिपोर्ट को PDF फ़ॉर्मेट में निर्दिष्ट फ़ाइल पथ पर सहेजता है।

```csharp
public void SaveReport(string fileName, ReportType reportType)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileName | स्ट्रिंग | निर्दिष्ट फ़ाइल नाम। |
| reportType | ReportType | निर्दिष्ट रिपोर्ट प्रकार।[`ReportType`](../../../aspose.tasks.visualization/reporttype/) |

## उदाहरण

दिखाता है कि प्रोजेक्ट रिपोर्ट को PDF फ़ॉर्मेट में कैसे सहेजा जाए।

```csharp
var project = new Project(DataDir + "OzBuild 16 Orig.mpp");
project.SaveReport(OutDir + "CostOverview_out.pdf", ReportType.CostOverview);
```

### संबंधित देखें

* enum [ReportType](../../../aspose.tasks.visualization/reporttype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


