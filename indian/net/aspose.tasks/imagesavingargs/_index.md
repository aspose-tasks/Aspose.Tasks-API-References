---
title: "Class ImageSavingArgs"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.ImageSavingArgs क्लास। यह क्लास बाहरी इमेज फ़ाइलों को सहेजने से संबंधित डेटा का सेट दर्शाती है जो HTML फ़ॉर्मेट में रूपांतरण के दौरान होता है।"
type: docs
weight: 900
url: /hi/net/aspose.tasks/imagesavingargs/
---
## ImageSavingArgs class

यह क्लास HTML फ़ॉर्मेट में रूपांतरण के दौरान बाहरी इमेज फ़ाइल के सहेजने से संबंधित डेटा सेट का प्रतिनिधित्व करती है।

```csharp
public class ImageSavingArgs : ResourceSavingArgs
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [ImageSavingArgs](imagesavingargs/)() | `ImageSavingArgs` क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [FileName](../../aspose.tasks/resourcesavingargs/filename/) { get; set; } | कनवर्टर से कस्टम मेथड के कोड तक जाने वाले अनुमानित फ़ाइल नाम को प्राप्त करता है या सेट करता है। इसे कस्टम कोड में यह तय करने के लिए उपयोग किया जा सकता है कि फ़ाइल को कैसे प्रोसेस किया जाए या कहाँ सहेजा जाए। |
| [ImageType](../../aspose.tasks/imagesavingargs/imagetype/) { get; } | एक HTML इमेज प्रकार प्राप्त करता है। |
| [KeepStreamOpen](../../aspose.tasks/resourcesavingargs/keepstreamopen/) { get; set; } | संसाधन सहेजने के समाप्त होने के बाद स्ट्रीम को खुला रखने का संकेत देने वाला मान प्राप्त करता है या सेट करता है। |
| [Stream](../../aspose.tasks/resourcesavingargs/stream/) { get; set; } | सहेजी गई फ़ाइल की बाइनरी सामग्री को प्राप्त करता है या सेट करता है। |
| [Uri](../../aspose.tasks/resourcesavingargs/uri/) { get; set; } | संसाधन URI को प्राप्त करता है या सेट करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [CloseStreamIfRequired](../../aspose.tasks/resourcesavingargs/closestreamifrequired/)() | यदि KeepStreamOpen false है तो स्ट्रीम बंद करें, अन्यथा इसे फ़्लश करें। |

## उदाहरण

इमेज सहेजने के आर्ग्युमेंट्स के साथ काम करने का तरीका दिखाता है।

```csharp
public void ResourcePrefixForNestedResourcesExample()
{
    var project = new Project(DataDir + "Project1.mpp");
    var options = ResourcePrefixForNestedResources.GetSaveOptions(1);
    project.Save(OutDir + "document_out.html", options);
}

private class ResourcePrefixForNestedResources : ICssSavingCallback, IFontSavingCallback, IImageSavingCallback
{
    public void CssSaving(CssSavingArgs args)
    {
        if (!Directory.Exists(OutDir + "css/"))
        {
            Directory.CreateDirectory(OutDir + "css/");
        }

        var stream = new FileStream(OutDir + "css/" + args.FileName, FileMode.Create);
        args.Stream = stream;
        args.KeepStreamOpen = false;
        args.Uri = OutDir + "css/" + args.FileName;
    }

    public void FontSaving(FontSavingArgs args)
    {
        if (!Directory.Exists(OutDir + "fonts/"))
        {
            Directory.CreateDirectory(OutDir + "fonts/");
        }

        var stream = new FileStream(OutDir + "fonts/" + args.FileName, FileMode.Create);
        args.Stream = stream;
        args.KeepStreamOpen = false;
        args.Uri = OutDir + "fonts/" + args.FileName;
    }

    public void ImageSaving(ImageSavingArgs args)
    {
        if (!Directory.Exists(OutDir + "resources/"))
        {
            Directory.CreateDirectory(OutDir + "resources/");
        }

        if (!Directory.Exists(OutDir + "resources/nestedResources/"))
        {
            Directory.CreateDirectory(OutDir + "resources/nestedResources/");
        }

        if (args.FileName.EndsWith("png"))
        {
            var stream1 = new FileStream(OutDir + "resources/nestedResources/" + args.FileName, FileMode.Create);
            args.Stream = stream1;
            args.KeepStreamOpen = false;
            args.Uri = OutDir + "resources/" + args.FileName;

            // args.NestedUri = dataDir + \"nestedResources/\" + args.FileName;
        }
        else
        {
            var stream2 = new FileStream(OutDir + "resources/" + args.FileName, FileMode.Create);
            args.Stream = stream2;
            args.KeepStreamOpen = false;
            args.Uri = OutDir + "resources/" + args.FileName;
        }
    }

    public static HtmlSaveOptions GetSaveOptions(int pageNumber)
    {
        var options = new HtmlSaveOptions
                          {
                              Pages = new List<int>(),
                              IncludeProjectNameInPageHeader = false,
                              IncludeProjectNameInTitle = false,
                              PageSize = PageSize.A3,
                              Timescale = Timescale.ThirdsOfMonths,
                              ReduceFooterGap = true,
                              FontFaceTypes = FontFaceType.Ttf,
                              ExportCss = ResourceExportType.AsFile,
                              ExportFonts = ResourceExportType.AsFile,
                              ExportImages = ResourceExportType.AsFile
                          };

        var program = new ResourcePrefixForNestedResources();
        options.FontSavingCallback = program;
        options.CssSavingCallback = program;
        options.ImageSavingCallback = program;

        options.Pages.Clear();
        options.Pages.Add(pageNumber);

        if (!Directory.Exists(DataDir + "fonts"))
        {
            Directory.CreateDirectory(DataDir + "fonts");
        }

        if (!Directory.Exists(DataDir + "resources"))
        {
            Directory.CreateDirectory(DataDir + "resources");
        }

        if (!Directory.Exists(DataDir + "nestedResources"))
        {
            Directory.CreateDirectory(DataDir + "resources/nestedResources");
        }

        if (!Directory.Exists(DataDir + "css"))
        {
            Directory.CreateDirectory(DataDir + "css");
        }

        return options;
    }
}
```

### संबंधित देखें

* class [ResourceSavingArgs](../resourcesavingargs/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


