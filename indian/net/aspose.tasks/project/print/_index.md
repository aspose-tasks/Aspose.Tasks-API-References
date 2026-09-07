---
title: "Project.Print"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project method. मानक बिना उपयोगकर्ता इंटरफ़ेस प्रिंट कंट्रोलर का उपयोग करके डिफ़ॉल्ट प्रिंटर सेटिंग्स के साथ प्रोजेक्ट को डिफ़ॉल्ट प्रिंटर पर प्रिंट करता है"
type: docs
weight: 1140
url: /hi/net/aspose.tasks/project/print/
---
## Print() {#print}

मानक (बिना उपयोगकर्ता इंटरफ़ेस) प्रिंट कंट्रोलर का उपयोग करके डिफ़ॉल्ट प्रिंटर सेटिंग्स के साथ परियोजना को डिफ़ॉल्ट प्रिंटर पर प्रिंट करता है।

```csharp
public void Print()
```

## उदाहरण

दिखाता है कि प्रोजेक्ट को कैसे प्रिंट किया जाए।

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Print();
```

### संबंधित देखें

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrintOptions) {#print_1}

मानक (बिना उपयोगकर्ता इंटरफ़ेस) प्रिंट कंट्रोलर का उपयोग करके डिफ़ॉल्ट प्रिंटर सेटिंग्स और कस्टम सहेजने विकल्पों के साथ परियोजना को डिफ़ॉल्ट प्रिंटर पर प्रिंट करता है।

```csharp
public void Print(PrintOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| options | PrintOptions | निर्दिष्ट [`PrintOptions`](../../../aspose.tasks.saving/printoptions/) क्लास की इंस्टेंस। |

## उदाहरण

दिखाता है कि प्रिंट विकल्पों का उपयोग करके प्रोजेक्ट को कैसे प्रिंट किया जाए।

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new PrintOptions
{
    Timescale = Timescale.ThirdsOfMonths
};
if (project.GetPageCount(Timescale.ThirdsOfMonths) <= 280)
{
    project.Print(options);
}
```

### संबंधित देखें

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(string) {#print_6}

मानक (बिना उपयोगकर्ता इंटरफ़ेस) प्रिंट कंट्रोलर का उपयोग करके डिफ़ॉल्ट प्रिंटर सेटिंग्स के साथ निर्दिष्ट प्रिंटर पर परियोजना को प्रिंट करता है।

```csharp
public void Print(string printerName)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| printerName | स्ट्रिंग | निर्दिष्ट प्रिंटर नाम। |

## उदाहरण

दिखाता है कि चयनित प्रिंटर पर प्रोजेक्ट को कैसे प्रिंट किया जाए।

```csharp
var project = new Project(DataDir + "Project2.mpp");

foreach (string printer in PrinterSettings.InstalledPrinters)
{
    if (!printer.ToUpperInvariant().Contains("Microsoft Print to PDF".ToUpperInvariant()))
    {
        continue;
    }

    project.Print(printer);
    break;
}
```

### संबंधित देखें

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings) {#print_2}

मानक (बिना उपयोगकर्ता इंटरफ़ेस) प्रिंट कंट्रोलर का उपयोग करके निर्दिष्ट प्रिंटर सेटिंग्स के अनुसार परियोजना को प्रिंट करता है।

```csharp
public void Print(PrinterSettings printerSettings)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| printerSettings | PrinterSettings | निर्दिष्ट PrinterSettings क्लास का उदाहरण। |

## उदाहरण

प्रोजेक्ट को प्रिंट करने के लिए प्रिंटर सेटिंग्स का उपयोग कैसे करें, दिखाता है।

```csharp
var project = new Project(DataDir + "Project2.mpp");

// पहले दो पृष्ठ प्रिंट करें
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings);
```

### संबंधित देखें

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, string) {#print_5}

मानक (बिना उपयोगकर्ता इंटरफ़ेस) प्रिंट कंट्रोलर का उपयोग करके निर्दिष्ट प्रिंटर सेटिंग्स के अनुसार परियोजना को प्रिंट करता है।

```csharp
public void Print(PrinterSettings printerSettings, string documentName)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| printerSettings | PrinterSettings | निर्दिष्ट PrinterSettings क्लास का उदाहरण। |
| documentName | स्ट्रिंग | दिखाने के लिए दस्तावेज़ का नाम (उदाहरण के लिए, प्रिंट स्थिति डायलॉग बॉक्स या प्रिंटर कतार में)। |

## उदाहरण

प्रोजेक्ट को प्रिंट करने के लिए प्रिंटर सेटिंग्स और दस्तावेज़ नाम का उपयोग कैसे करें, दिखाता है।

```csharp
var project = new Project(DataDir + "Project2.mpp");

// पहले दो पृष्ठ प्रिंट करें
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, "Document #1");
```

### संबंधित देखें

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, PrintOptions) {#print_3}

मानक (बिना उपयोगकर्ता इंटरफ़ेस) प्रिंट कंट्रोलर का उपयोग करके निर्दिष्ट प्रिंटर सेटिंग्स और कस्टम सहेजने विकल्पों के अनुसार परियोजना को प्रिंट करता है।

```csharp
public void Print(PrinterSettings printerSettings, PrintOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| printerSettings | PrinterSettings | निर्दिष्ट PrinterSettings क्लास का उदाहरण। |
| options | PrintOptions | निर्दिष्ट [`PrintOptions`](../../../aspose.tasks.saving/printoptions/) क्लास की इंस्टेंस। |

## उदाहरण

प्रोजेक्ट को प्रिंट करने के लिए प्रिंटर विकल्प और सेटिंग्स का उपयोग कैसे करें, दिखाता है।

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new PrintOptions
{
    Timescale = Timescale.Months
};

// पहले दो पृष्ठ प्रिंट करें
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, options);
```

### संबंधित देखें

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, PrintOptions, string) {#print_4}

मानक (बिना उपयोगकर्ता इंटरफ़ेस) प्रिंट कंट्रोलर का उपयोग करके निर्दिष्ट प्रिंटर सेटिंग्स, कस्टम सहेजने विकल्प और निर्दिष्ट दस्तावेज़ नाम के अनुसार परियोजना को प्रिंट करता है।

```csharp
public void Print(PrinterSettings printerSettings, PrintOptions options, string documentName)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| printerSettings | PrinterSettings | निर्दिष्ट PrinterSettings क्लास का उदाहरण। |
| options | PrintOptions | निर्दिष्ट [`PrintOptions`](../../../aspose.tasks.saving/printoptions/) क्लास की इंस्टेंस। |
| documentName | स्ट्रिंग | दिखाने के लिए दस्तावेज़ का नाम (उदाहरण के लिए, प्रिंट स्थिति डायलॉग बॉक्स या प्रिंटर कतार में)। |

## उदाहरण

प्रोजेक्ट को प्रिंट करने के लिए प्रिंटर विकल्प, प्रिंटर सेटिंग्स और दस्तावेज़ नाम का उपयोग कैसे करें, दिखाता है।

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new PrintOptions
{
    Timescale = Timescale.Months
};

// पहले दो पृष्ठ प्रिंट करें
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, options, "My project name");
```

### संबंधित देखें

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


