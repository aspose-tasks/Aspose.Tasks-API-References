---
title: GetPageCount
second_title: Aspose.Tasks for .NET API Reference
description: दए गए क उपयग करके प्रस्तुत कए जने वले प्रजेक्ट के लए पृष्ठ संख्य लटत हैSaveOptionsaspose.tasks.saving/saveoptions/ .
type: docs
weight: 1080
url: /hi/net/aspose.tasks/project/getpagecount/
---
## GetPageCount(SaveOptions) {#getpagecount_1}

दिए गए का उपयोग करके प्रस्तुत किए जाने वाले प्रोजेक्ट के लिए पृष्ठ संख्या लौटाता है[`SaveOptions`](../../../aspose.tasks.saving/saveoptions/) .

```csharp
public int GetPageCount(SaveOptions saveOptions)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| saveOptions | SaveOptions | पृष्ठों की संख्या प्राप्त करने के लिए सहेजें विकल्प। |

### प्रतिलाभ की मात्रा

प्रदान किए जाने वाले पृष्ठ की संख्या।

### उदाहरण

इस उदाहरण में HtmlSaveOptions और परिणामी HTML में पृष्ठों की संख्या कंसोल पर लिखी गई है।

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

### यह सभी देखें

* class [SaveOptions](../../../aspose.tasks.saving/saveoptions/)
* class [Project](../)
* नाम स्थान [Aspose.Tasks](../../project/)
* सभा [Aspose.Tasks](../../../)

---

## GetPageCount() {#getpagecount}

डिफ़ॉल्ट रूप से प्रस्तुत किए जाने वाले प्रोजेक्ट के लिए पृष्ठ संख्या लौटाता है[`Timescale`](../../../aspose.tasks.visualization/timescale/) (दिन).

```csharp
public int GetPageCount()
```

### प्रतिलाभ की मात्रा

रेंडर किए जाने वाले पेज की गिनती.

### यह सभी देखें

* class [Project](../)
* नाम स्थान [Aspose.Tasks](../../project/)
* सभा [Aspose.Tasks](../../../)

---

## GetPageCount(Timescale) {#getpagecount_6}

दिए गए का उपयोग करके प्रस्तुत किए जाने वाले प्रोजेक्ट के लिए पृष्ठ संख्या लौटाता है[`Timescale`](../../../aspose.tasks.visualization/timescale/) .

```csharp
public int GetPageCount(Timescale scale)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| scale | Timescale | पृष्ठ संख्या प्राप्त करने का पैमाना। |

### प्रतिलाभ की मात्रा

रेंडर किए जाने वाले पेज की गिनती.

### यह सभी देखें

* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* नाम स्थान [Aspose.Tasks](../../project/)
* सभा [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat) {#getpagecount_4}

डिफ़ॉल्ट रूप से प्रस्तुत किए जाने वाले प्रोजेक्ट के लिए पृष्ठ संख्या लौटाता है[`Timescale`](../../../aspose.tasks.visualization/timescale/) (दिन) और दिया[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/)

```csharp
public int GetPageCount(PresentationFormat format)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| format | PresentationFormat | पृष्ठ संख्या प्राप्त करने के लिए प्रारूप। |

### प्रतिलाभ की मात्रा

रेंडर किए जाने वाले पेज की गिनती.

### यह सभी देखें

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* class [Project](../)
* नाम स्थान [Aspose.Tasks](../../project/)
* सभा [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat, Timescale) {#getpagecount_5}

दिए गए का उपयोग करके प्रस्तुत किए जाने वाले प्रोजेक्ट के लिए पृष्ठ संख्या लौटाता है[`Timescale`](../../../aspose.tasks.visualization/timescale/) और[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) .

```csharp
public int GetPageCount(PresentationFormat format, Timescale scale)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| format | PresentationFormat | पृष्ठ संख्या प्राप्त करने के लिए प्रारूप। |
| scale | Timescale | पृष्ठ संख्या प्राप्त करने का पैमाना। |

### प्रतिलाभ की मात्रा

प्रदान किए जाने वाले पृष्ठ की संख्या।

### यह सभी देखें

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* नाम स्थान [Aspose.Tasks](../../project/)
* सभा [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale, DateTime, DateTime) {#getpagecount_3}

दिए गए का उपयोग करके प्रस्तुत किए जाने वाले प्रोजेक्ट के लिए पृष्ठ संख्या लौटाता है[`Timescale`](../../../aspose.tasks.visualization/timescale/) ,[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) और दिनांक सीमा.

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale, DateTime startDate, DateTime endDate)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pageSize | PageSize | पृष्ठ संख्या प्राप्त करने के लिए आकार। |
| scale | Timescale | पृष्ठ संख्या प्राप्त करने का पैमाना। |
| startDate | DateTime | पृष्ठ गणना प्राप्त करने की प्रारंभ तिथि। |
| endDate | DateTime | पृष्ठ संख्या प्राप्त करने की अंतिम तिथि। |

### प्रतिलाभ की मात्रा

रेंडर किए जाने वाले पेज की गिनती.

### यह सभी देखें

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* नाम स्थान [Aspose.Tasks](../../project/)
* सभा [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale) {#getpagecount_2}

दिए गए का उपयोग करके प्रस्तुत किए जाने वाले प्रोजेक्ट के लिए पृष्ठ संख्या लौटाता है[`Timescale`](../../../aspose.tasks.visualization/timescale/) और[`PageSize`](../../../aspose.tasks.visualization/pagesize/) .

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pageSize | PageSize | पृष्ठ संख्या प्राप्त करने के लिए आकार। |
| scale | Timescale | पृष्ठ संख्या प्राप्त करने का पैमाना। |

### प्रतिलाभ की मात्रा

रेंडर किए जाने वाले पेज की गिनती.

### यह सभी देखें

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* नाम स्थान [Aspose.Tasks](../../project/)
* सभा [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
