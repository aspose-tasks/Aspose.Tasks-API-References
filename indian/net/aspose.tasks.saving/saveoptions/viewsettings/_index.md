---
title: "SaveOptions.ViewSettings"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "SaveOptions प्रॉपर्टी। यह रेंडर करने के लिए एक View प्राप्त करता है या सेट करता है। आप इस विकल्प का उपयोग करके स्पष्ट रूप से निर्दिष्ट कर सकते हैं कि कौन सा view PDF, HTML या Image फ़ॉर्मेट में सहेजा जाना चाहिए। यदि यह प्रॉपर्टी सेट है तो PresentationFormat प्रॉपर्टी को प्रोजेक्ट सहेजे जाने पर अनदेखा किया जाता है। View को निम्नलिखित स्क्रीन में से किसी एक से होना चाहिए: Screen, Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage।"
type: docs
weight: 240
url: /hi/net/aspose.tasks.saving/saveoptions/viewsettings/
---
## SaveOptions.ViewSettings property

एक view ([`View`](../view/)) प्राप्त करता है या सेट करता है जिसे रेंडर किया जाएगा। आप इस विकल्प का उपयोग करके स्पष्ट रूप से निर्दिष्ट कर सकते हैं कि कौन सा view PDF, HTML या Image फ़ॉर्मेट में सहेजा जाना चाहिए। यदि यह प्रॉपर्टी सेट है, तो [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) प्रॉपर्टी को प्रोजेक्ट सहेजे जाने पर अनदेखा किया जाता है। View को निम्नलिखित स्क्रीन में से किसी एक से होना चाहिए (([`Screen`](../../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)।

```csharp
public View ViewSettings { get; set; }
```

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentException | जब सेट मेथड को कॉल किया जाता है और View क्लास का एक इंस्टेंस जिसमें Screen प्रॉपर्टी का असमर्थित मान दिया गया है, प्रदान किया जाता है। |

## उदाहरण

दिखाता है कि 'SaveOptions.ViewSettings' का उपयोग करके वह view कैसे निर्दिष्ट किया जाए जिसे PDF में रेंडर किया जाना चाहिए।

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);
Console.WriteLine("Page size specified in view settings: " + view.PageInfo.PageSettings.PaperSize);
Console.WriteLine("Page orientation: {0}", view.PageInfo.PageSettings.IsPortrait ? "Portrait" : "Landscape");

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSize = PageSize.DefinedInView;
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.StartDate = new DateTime(2012, 12, 22);
saveOptions.EndDate = new DateTime(2013, 05, 10);
saveOptions.ViewSettings = view;

project.Save(OutDir + "SaveToPdfUsingSpecificView_out.pdf", saveOptions);
```

### संबंधित देखें

* class [View](../../../aspose.tasks/view/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


