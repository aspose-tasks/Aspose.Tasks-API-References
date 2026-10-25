---
title: "ProjectDisplayOptions.MonthLabel"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ProjectDisplayOptions प्रॉपर्टी। महीने के लेबल के प्रदर्शित होने का तरीका प्राप्त करता है या सेट करता है"
type: docs
weight: 60
url: /hi/net/aspose.tasks/projectdisplayoptions/monthlabel/
---
## ProjectDisplayOptions.MonthLabel property

महीना लेबल कैसे प्रदर्शित होता है, इसे प्राप्त करता है या सेट करता है।

```csharp
public MonthLabelDisplay MonthLabel { get; set; }
```

## उदाहरण

प्रोजेक्ट के डिस्प्ले विकल्पों का उपयोग कैसे करें, यह दिखाता है।

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// प्रोजेक्ट द्वारा मैन्युअल रूप से निर्धारित कार्य में संभावित शेड्यूलिंग टकराव की पहचान होने पर चेतावनियाँ दिखाने के लिए मान सेट करें।
// यह विकल्प प्रोजेक्ट 2010 संस्करण और बाद के संस्करणों के लिए उपलब्ध है।
project.DisplayOptions.ShowTaskScheduleWarnings = false;

// संख्या मान और समय संक्षिप्ताक्षर (1 wk बनाम 1wk) के पहले एक स्पेस जोड़ने के लिए संकेत देने वाला मान।
project.DisplayOptions.AddSpaceBeforeLabel = true;

// मिनट लेबल कैसे प्रदर्शित होता है, इसे सेट करें
project.DisplayOptions.MinuteLabel = MinuteLabelDisplay.Min;

// घंटे लेबल के प्रदर्शित होने का तरीका सेट करें।
project.DisplayOptions.HourLabel = HourLabelDisplay.Hr;

// दिन लेबल कैसे प्रदर्शित होता है, इसे सेट करें।
project.DisplayOptions.DayLabel = DayLabelDisplay.Dy;

// सप्ताह लेबल कैसे प्रदर्शित होता है, इसे सेट करें।
project.DisplayOptions.WeekLabel = WeekLabelDisplay.Week;

// महीने का लेबल कैसे प्रदर्शित होता है, सेट करें
project.DisplayOptions.MonthLabel = MonthLabelDisplay.Mon;

// वर्ष लेबल कैसे प्रदर्शित किया जाता है, सेट करें
project.DisplayOptions.YearLabel = YearLabelDisplay.Year;

// गैंट चार्ट दृश्य के शीर्ष पर अपने स्वयं के सारांश कार्य बार के साथ एक पंक्ति में पूरे प्रोजेक्ट की सारांश जानकारी प्रदर्शित करने के लिए संकेत देने वाला मान सेट करें।
project.DisplayOptions.ShowProjectSummaryTask = true;

// प्रोजेक्ट द्वारा मैन्युअल रूप से निर्धारित कार्य में संभावित शेड्यूलिंग टकराव की पहचान होने पर सुझाव दिखाने के लिए संकेत देने वाला मान सेट करें।
project.DisplayOptions.ShowTaskScheduleSuggestions = true;

// हाइपरलिंक को रेखांकित करने के लिए संकेत देने वाला मान सेट करें।
project.DisplayOptions.UnderlineHyperlinks = true;

project.Save(OutDir + "WorkWithProjectDisplayOptions.mpp", SaveFileFormat.Mpp);
```

### संबंधित देखें

* enum [MonthLabelDisplay](../../monthlabeldisplay/)
* class [ProjectDisplayOptions](../)
* namespace [Aspose.Tasks](../../projectdisplayoptions/)
* assembly [Aspose.Tasks](../../../)


