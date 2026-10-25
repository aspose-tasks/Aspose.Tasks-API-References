---
title: "क्लास NoPrinterInstalledException"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.NoPrinterInstalledException क्लास। जब ऑपरेटिंग सिस्टम में कोई प्रिंटर स्थापित नहीं होता है, तब फेंकी जाने वाली अपवाद को दर्शाता है।"
type: docs
weight: 1100
url: /hi/net/aspose.tasks/noprinterinstalledexception/
---
## NoPrinterInstalledException class

ऑपरेटिंग सिस्टम में कोई स्थापित प्रिंटर न होने पर फेंकी जाने वाली अपवाद का प्रतिनिधित्व करता है।

```csharp
public class NoPrinterInstalledException : Exception
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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


