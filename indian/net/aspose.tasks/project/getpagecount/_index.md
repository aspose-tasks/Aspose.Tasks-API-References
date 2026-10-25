---
title: "Project.GetPageCount"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project मेथड। दिए गए SaveOptions का उपयोग करके रेंडर किए जाने वाले प्रोजेक्ट के लिए पृष्ठ गिनती लौटाता है।"
type: docs
weight: 1110
url: /hi/net/aspose.tasks/project/getpagecount/
---
## GetPageCount(SaveOptions) {#getpagecount_1}

दिए गए [`SaveOptions`](../../../aspose.tasks.saving/saveoptions/) का उपयोग करके रेंडर किए जाने वाले प्रोजेक्ट के लिए पृष्ठ गिनती लौटाता है।

```csharp
public int GetPageCount(SaveOptions saveOptions)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| saveOptions | SaveOptions | पृष्ठ गिनती प्राप्त करने के लिए सहेजने के विकल्प। |

### रिटर्न वैल्यू

रेंडर किए जाने के लिए पृष्ठ गिनती।

## उदाहरण

इस उदाहरण में HtmlSaveOptions का इंस्टेंस और परिणामी HTML में पृष्ठों की संख्या कंसोल में लिखी जाती है।

```csharp
[C#]
Project project = new Project(@"test.mpp");
HtmlSaveOptions saveOptions = new HtmlSaveOptions
{
    IncludeProjectNameInPageHeader = false,
    IncludeProjectNameInTitle = false,
    PageSize = PageSize.A4,
    Timescale = Timescale.Days,
    StartDate = project.Get(Prj.StartDate).Date,
    EndDate = project.Get(Prj.FinishDate).Date
};

Console.WriteLine(project.GetPageCount(saveOptions));
```

विशिष्ट सहेजने के विकल्पों के लिए पृष्ठ गिनती प्राप्त करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");
var options = new HtmlSaveOptions
                  {
                      IncludeProjectNameInPageHeader = false,
                      IncludeProjectNameInTitle = false,
                      PageSize = PageSize.A4,
                      Timescale = Timescale.Days,
                      StartDate = project.Get(Prj.StartDate).Date,
                      EndDate = project.Get(Prj.FinishDate).Date
                  };

Console.WriteLine(project.GetPageCount(options));
```

### संबंधित देखें

* class [SaveOptions](../../../aspose.tasks.saving/saveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount() {#getpagecount}

डिफ़ॉल्ट [`Timescale`](../../../aspose.tasks.visualization/timescale/)(Days) का उपयोग करके रेंडर किए जाने वाले प्रोजेक्ट के लिए पृष्ठ गिनती लौटाता है।

```csharp
public int GetPageCount()
```

### रिटर्न वैल्यू

रेंडर की जाने वाली पृष्ठ गिनती।

## उदाहरण

विभिन्न टाइमस्केल के लिए पृष्ठ गिनती प्राप्त करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");

// पृष्ठों की संख्या प्राप्त करें, Timescale.Months, Timescale.ThirdsOfMonths
var pageCount = project.GetPageCount();
Console.WriteLine("Page count: " + pageCount);
pageCount = project.GetPageCount(Timescale.Months);
Console.WriteLine("Page count (Month): " + pageCount);
pageCount = project.GetPageCount(Timescale.ThirdsOfMonths);
Console.WriteLine("Page count (Thirds of Months): " + pageCount);
```

### संबंधित देखें

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(Timescale) {#getpagecount_6}

दिए गए [`Timescale`](../../../aspose.tasks.visualization/timescale/) का उपयोग करके रेंडर किए जाने वाले प्रोजेक्ट के लिए पृष्ठ गिनती लौटाता है।

```csharp
public int GetPageCount(Timescale scale)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| स्केल | टाइमस्केल | पृष्ठ गिनती प्राप्त करने के लिए स्केल। |

### रिटर्न वैल्यू

रेंडर की जाने वाली पृष्ठ गिनती।

## उदाहरण

विभिन्न टाइमस्केल के लिए पृष्ठ गिनती प्राप्त करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");

// पृष्ठों की संख्या प्राप्त करें, Timescale.Months, Timescale.ThirdsOfMonths
var pageCount = project.GetPageCount();
Console.WriteLine("Page count: " + pageCount);
pageCount = project.GetPageCount(Timescale.Months);
Console.WriteLine("Page count (Month): " + pageCount);
pageCount = project.GetPageCount(Timescale.ThirdsOfMonths);
Console.WriteLine("Page count (Thirds of Months): " + pageCount);
```

### संबंधित देखें

* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat) {#getpagecount_4}

डिफ़ॉल्ट [`Timescale`](../../../aspose.tasks.visualization/timescale/)(Days) और दिए गए [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) का उपयोग करके रेंडर किए जाने वाले प्रोजेक्ट के लिए पृष्ठ गिनती लौटाता है।

```csharp
public int GetPageCount(PresentationFormat format)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| फ़ॉर्मेट | प्रेजेंटेशनफ़ॉर्मेट | पृष्ठ गिनती प्राप्त करने के लिए फ़ॉर्मेट। |

### रिटर्न वैल्यू

रेंडर की जाने वाली पृष्ठ गिनती।

## उदाहरण

प्रेजेंटेशन फ़ॉर्मेट और टाइमस्केल द्वारा पृष्ठों की गिनती प्राप्त करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "GetNumberOfPagesForViews.mpp");

// डिफ़ॉल्ट रूप से Days, Months और ThirdsOfMonths के लिए पृष्ठों की संख्या प्राप्त करें
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Days));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Months));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.ThirdsOfMonths));
```

### संबंधित देखें

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat, Timescale) {#getpagecount_5}

दिए गए [`Timescale`](../../../aspose.tasks.visualization/timescale/) और [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) का उपयोग करके रेंडर किए जाने वाले प्रोजेक्ट के लिए पृष्ठ गिनती लौटाता है।

```csharp
public int GetPageCount(PresentationFormat format, Timescale scale)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| फ़ॉर्मेट | प्रेजेंटेशनफ़ॉर्मेट | पृष्ठ गिनती प्राप्त करने के लिए फ़ॉर्मेट। |
| स्केल | टाइमस्केल | पृष्ठ गिनती प्राप्त करने के लिए स्केल। |

### रिटर्न वैल्यू

रेंडर किए जाने के लिए पृष्ठ गिनती।

## उदाहरण

प्रेजेंटेशन फ़ॉर्मेट और टाइमस्केल द्वारा पृष्ठों की गिनती प्राप्त करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "GetNumberOfPagesForViews.mpp");

// डिफ़ॉल्ट रूप से Days, Months और ThirdsOfMonths के लिए पृष्ठों की संख्या प्राप्त करें
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Days));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Months));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.ThirdsOfMonths));
```

### संबंधित देखें

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale, DateTime, DateTime) {#getpagecount_3}

दिए गए [`Timescale`](../../../aspose.tasks.visualization/timescale/), [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) और तिथि सीमा का उपयोग करके रेंडर किए जाने वाले प्रोजेक्ट के लिए पृष्ठ गिनती लौटाता है।

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale, DateTime startDate, DateTime endDate)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pageSize | PageSize | पृष्ठ गिनती प्राप्त करने के लिए आकार। |
| स्केल | टाइमस्केल | पृष्ठ गिनती प्राप्त करने के लिए स्केल। |
| startDate | DateTime | पृष्ठ गिनती प्राप्त करने के लिए प्रारंभ तिथि। |
| endDate | DateTime | पृष्ठ गिनती प्राप्त करने के लिए समाप्ति तिथि। |

### रिटर्न वैल्यू

रेंडर की जाने वाली पृष्ठ गिनती।

## उदाहरण

पृष्ठ आकार, टाइमस्केल, प्रारंभ और समाप्ति तिथियों द्वारा पृष्ठों की गिनती प्राप्त करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");
var pageCount = project.GetPageCount(
    PageSize.A3,
    Timescale.Months,
    project.Get(Prj.StartDate) - TimeSpan.FromDays(10),
    project.Get(Prj.FinishDate) + TimeSpan.FromDays(30));

Console.WriteLine(pageCount);
```

### संबंधित देखें

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale) {#getpagecount_2}

दिए गए [`Timescale`](../../../aspose.tasks.visualization/timescale/) और [`PageSize`](../../../aspose.tasks.visualization/pagesize/) का उपयोग करके रेंडर किए जाने वाले प्रोजेक्ट के लिए पृष्ठ गिनती लौटाता है।

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pageSize | PageSize | पृष्ठ गिनती प्राप्त करने के लिए आकार। |
| स्केल | टाइमस्केल | पृष्ठ गिनती प्राप्त करने के लिए स्केल। |

### रिटर्न वैल्यू

रेंडर की जाने वाली पृष्ठ गिनती।

## उदाहरण

पृष्ठ आकार और समय स्केल द्वारा पृष्ठों की गिनती प्राप्त करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");
var pageCount = project.GetPageCount(PageSize.A3, Timescale.Months);

Console.WriteLine(pageCount);
```

### संबंधित देखें

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


