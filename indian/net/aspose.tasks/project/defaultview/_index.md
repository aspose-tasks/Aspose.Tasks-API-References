---
title: "Project.DefaultView"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project प्रॉपर्टी। प्रोजेक्ट का डिफ़ॉल्ट व्यू प्राप्त करता है या सेट करता है।"
type: docs
weight: 360
url: /hi/net/aspose.tasks/project/defaultview/
---
## Project.DefaultView property

परियोजना का डिफ़ॉल्ट दृश्य प्राप्त करता है या सेट करता है।

```csharp
public View DefaultView { get; set; }
```

## उदाहरण

प्रोजेक्ट के डिफ़ॉल्ट व्यू के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "TaskUsageViewWithDetails.mpp");

// डिफ़ॉल्ट व्यू प्राप्त करें
UsageView view = (TaskUsageView)project.DefaultView;

// डिटेल्स हेडर कॉलम प्रदर्शित नहीं होगा
view.DisplayDetailsHeaderColumn = false;
view.RepeatDetailsHeaderOnAllRows = false;
view.AlignDetailsData = HorizontalStringAlignment.Near;
project.Save(OutDir + "task usage1_out.pdf", SaveFileFormat.Pdf);

// डिटेल्स हेडर कॉलम प्रदर्शित करें
view.DisplayDetailsHeaderColumn = true;

// सभी असाइनमेंट पंक्तियों पर डिटेल्स हेडर दोहराएँ
view.RepeatDetailsHeaderOnAllRows = true;
view.AlignDetailsData = HorizontalStringAlignment.Far;
project.Save(OutDir + "task usage2_out.pdf", SaveFileFormat.Pdf);
```

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

### संबंधित देखें

* class [View](../../view/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


