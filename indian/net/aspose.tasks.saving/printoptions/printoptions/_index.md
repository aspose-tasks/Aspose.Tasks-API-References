---
title: "PrintOptions.PrintOptions"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PrintOptions constructor. नई PrintOptions क्लास की एक नई इंस्टेंस को इनिशियलाइज़ करता है जिसे प्रोजेक्ट प्रिंट करने के विभिन्न विकल्प सेट करने के लिए उपयोग किया जा सकता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks.saving/printoptions/printoptions/
---
## PrintOptions constructor

नई [`PrintOptions`](../) क्लास की एक नई इंस्टेंस को इनिशियलाइज़ करता है जिसे प्रोजेक्ट प्रिंट करने के विभिन्न विकल्प सेट करने के लिए उपयोग किया जा सकता है।

```csharp
public PrintOptions()
```

## उदाहरण

प्रिंट विकल्पों का उपयोग कैसे करें, यह दर्शाता है।

```csharp
try
{
    var project = new Project(DataDir + "Project2.mpp");
    var options = new PrintOptions
    {
        Timescale = Timescale.ThirdsOfMonths
    };
    if (project.GetPageCount(Timescale.ThirdsOfMonths) <= 280)
    {
        project.Print(options);
    }
}
catch (NoPrinterInstalledException ex)
{
    Console.WriteLine(ex.Message);
}
```

### संबंधित देखें

* class [PrintOptions](../)
* namespace [Aspose.Tasks.Saving](../../printoptions/)
* assembly [Aspose.Tasks](../../../)


