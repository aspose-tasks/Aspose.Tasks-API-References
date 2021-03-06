---
title: ViewSettings
second_title: Aspose.Tasks for .NET API Reference
description: 
type: docs
weight: 230
url: /net/aspose.tasks.saving/saveoptions/viewsettings/
---
## SaveOptions.ViewSettings property

Gets or sets a view ([`View`](../view)) to render. You can use this options to explicitly specify which view should be saved to PDF, HTML or Image formats. If this property is set, [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat) property is ignored when project is saved. View should be from one of the following screen (([`Screen`](../../../aspose.tasks/view/screen))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)

```csharp
public View ViewSettings { get; set; }
```

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | When set method is called and instance of View class with not supported value of Screen property is provided. |

### See Also

* class [View](../../../aspose.tasks/view)
* class [SaveOptions](../../saveoptions)
* namespace [Aspose.Tasks.Saving](../../saveoptions)
* assembly [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
