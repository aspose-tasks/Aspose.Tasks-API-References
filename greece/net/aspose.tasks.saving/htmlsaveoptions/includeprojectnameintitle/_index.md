---
title: "HtmlSaveOptions.IncludeProjectNameInTitle"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα HtmlSaveOptions. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα συμπεριληφθεί το όνομα του έργου στον τίτλο HTML."
type: docs
weight: 120
url: /el/net/aspose.tasks.saving/htmlsaveoptions/includeprojectnameintitle/
---
## HtmlSaveOptions.IncludeProjectNameInTitle property

Αποκτά ή ορίζει μια τιμή που υποδεικνύει εάν θα συμπεριληφθεί το όνομα του έργου στον τίτλο της HTML.

```csharp
public bool IncludeProjectNameInTitle { get; set; }
```

## Παραδείγματα

Δείχνει πώς να ορίσετε την κεφαλίδα/τίτλο HTML της σελίδας χρησιμοποιώντας τις επιλογές &lt;see cref=\"P:Aspose.Tasks.Saving.HtmlSaveOptions\" /&gt;.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new HtmlSaveOptions
{
    // Καθορίζει εάν θα συμπεριληφθεί το όνομα του έργου στον τίτλο HTML (αληθές εξ ορισμού)
    IncludeProjectNameInTitle = false,

    // Καθορίζει εάν θα συμπεριληφθεί το όνομα του έργου στην κεφαλίδα σελίδας HTML (αληθές εξ ορισμού)
    IncludeProjectNameInPageHeader = false,

    // ορίστε τις σελίδες που θα εξαχθούν
    Pages = new List<int>
            {
                1
            }
};
project.Save(OutDir + "ControlHeaderNameDuringHTMLExport_out.html", options);
```

### Δείτε επίσης

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


