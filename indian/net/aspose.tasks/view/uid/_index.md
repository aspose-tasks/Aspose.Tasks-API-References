---
title: "View.Uid"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "View प्रॉपर्टी. एक दृश्य का अद्वितीय पहचानकर्ता प्राप्त करता है"
type: docs
weight: 120
url: /hi/net/aspose.tasks/view/uid/
---
## View.Uid property

एक दृश्य का अद्वितीय पहचानकर्ता प्राप्त करता है।

```csharp
public int Uid { get; }
```

## उदाहरण

प्रोजेक्ट के व्यू के साथ काम करने और डिफ़ॉल्ट व्यू में कॉलम जोड़ने का तरीका दिखाता है (जो MPP फ़ाइल को MS Project में खोलने पर दिखाया जाता है)।

```csharp
// व्यूज़ के बिना एक खाली प्रोजेक्ट बनाएं
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// डिफ़ॉल्ट व्यू को संशोधित करें (यह एक गैंट चार्ट व्यू है)।
// या आप प्रोजेक्ट.View संग्रह का उपयोग करके व्यू को नाम से या व्यू स्क्रीन से चुन सकते हैं।
var view = (GanttChartView) project.DefaultView;

TableField newColumn = new TableField()
{
    AlignData = HorizontalStringAlignment.Center,
    Title = "My new column",
    Width = 30,
    Field = Field.TaskActualDuration
};

view.Table.TableFields.Add(newColumn);

// WriteViewData फ़्लैग का उपयोग व्यू की प्रॉपर्टीज़ में किए गए बदलावों को स्थायी बनाने के लिए किया जाना चाहिए।
project.Save(OutDir + "ModifyView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
```

MS Project व्यूज़ के साथ काम करने का तरीका दिखाता है।

```csharp
// व्यूज़ के बिना एक खाली प्रोजेक्ट बनाएं
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// एक मानक गैंट चार्ट व्यू बनाएं
View view = new GanttChartView();

// कुछ व्यू प्रॉपर्टीज़ सेट करें
// Microsoft Project रिबन में व्यू या अन्य व्यूज़ ड्रॉप-डाउन सूची में एकल व्यू नाम दिखाता है या नहीं, यह दर्शाने वाला मान सेट करें
view.ShowInMenu = true;
// Microsoft Project एकल व्यू के लिए फ़िल्टर को हाइलाइट करता है या नहीं, यह दर्शाने वाला मान सेट करें
view.HighlightFilter = true;

// अगली प्रॉपर्टीज़ का लेखन समर्थित नहीं है
// एकल व्यू में उपयोग किए जाने वाले फ़िल्टर को सेट करता है
view.Filter = null;
// एकल व्यू का समूह सेट करता है
view.Group = null;
// एकल व्यू की टेबल सेट करता है
view.Table = null;

// आइए कुछ व्यू सेटिंग्स को ट्यून करें
// सभी पृष्ठों पर प्रिंट होने वाले पहले कॉलमों की संख्या सेट करें
view.PageInfo.PageViewSettings.FirstColumnsCount = 4;
// सभी पृष्ठों पर निर्दिष्ट संख्या में पहले कॉलम प्रिंट करने का संकेत देने वाला मान सेट करें
view.PageInfo.PageViewSettings.PrintFirstColumnsCountOnAllPages = true;

// व्यू को हमारे प्रोजेक्ट में जोड़ें
project.Views.Add(view);

// project.Views में संशोधनों को स्थायी रखने के लिए WriteViewData फ़्लैग का उपयोग किया जाना चाहिए।
project.Save(OutDir + "WorkWithView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
// आइए नए जोड़े गए व्यू की कुछ प्रॉपर्टीज़ जांचें
// व्यू का यूनिक आइडेंटिफायर प्रिंट करें
Console.WriteLine("View Uid: " + view.Uid);
// एकल व्यू के स्क्रीन टाइप को प्रिंट करें
Console.WriteLine("View Screen: " + view.Screen);
Console.WriteLine("View Type: " + view.Type);
Console.WriteLine("Parent Project of the view: " + view.ParentProject.Get(Prj.Name));
```

### संबंधित देखें

* class [View](../)
* namespace [Aspose.Tasks](../../view/)
* assembly [Aspose.Tasks](../../../)


