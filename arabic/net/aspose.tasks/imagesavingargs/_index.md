---
title: "Class ImageSavingArgs"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.ImageSavingArgs. تمثل هذه الفئة مجموعة من البيانات المتعلقة بحفظ ملفات الصور الخارجية التي تحدث أثناء التحويل إلى تنسيق HTML"
type: docs
weight: 900
url: /ar/net/aspose.tasks/imagesavingargs/
---
## ImageSavingArgs class

هذه الفئة تمثل مجموعة من البيانات المتعلقة بحفظ ملفات الصور الخارجية التي تحدث أثناء التحويل إلى تنسيق HTML.

```csharp
public class ImageSavingArgs : ResourceSavingArgs
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [ImageSavingArgs](imagesavingargs/)() | يُنشئ مثلاً جديداً من الفئة `ImageSavingArgs`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [FileName](../../aspose.tasks/resourcesavingargs/filename/) { get; set; } | يحصل أو يعيّن اسم الملف المفترض الذي ينتقل من المحوّل إلى شفرة الطريقة المخصّصة. يمكن استخدامه في الشفرة المخصّصة لتحديد كيفية معالجة الملف أو أين يتم حفظه. |
| [ImageType](../../aspose.tasks/imagesavingargs/imagetype/) { get; } | يحصل على نوع صورة HTML. |
| [KeepStreamOpen](../../aspose.tasks/resourcesavingargs/keepstreamopen/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان سيتم إبقاء الدفق مفتوحًا بعد انتهاء حفظ المورد. |
| [Stream](../../aspose.tasks/resourcesavingargs/stream/) { get; set; } | يحصل أو يعيّن المحتوى الثنائي للملف المحفوظ. |
| [Uri](../../aspose.tasks/resourcesavingargs/uri/) { get; set; } | يحصل أو يعيّن عنوان URI للمورد. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [CloseStreamIfRequired](../../aspose.tasks/resourcesavingargs/closestreamifrequired/)() | أغلق الدفق إذا كانت KeepStreamOpen خاطئة، وإلا قم بتفريغه. |

## الأمثلة

يظهر كيفية العمل مع معلمات حفظ الصورة.

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

### انظر أيضًا

* class [ResourceSavingArgs](../resourcesavingargs/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


