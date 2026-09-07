---
title: "क्लास ProjectDisplayOptions"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.ProjectDisplayOptions क्लास। प्रोजेक्ट इंस्टेंस के डिस्प्ले विकल्पों को दर्शाती है"
type: docs
weight: 1450
url: /hi/net/aspose.tasks/projectdisplayoptions/
---
## ProjectDisplayOptions class

एक प्रोजेक्ट इंस्टेंस के डिस्प्ले विकल्पों का प्रतिनिधित्व करता है।

```csharp
public class ProjectDisplayOptions
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [ProjectDisplayOptions](projectdisplayoptions/)() | `ProjectDisplayOptions` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [AddSpaceBeforeLabel](../../aspose.tasks/projectdisplayoptions/addspacebeforelabel/) { get; set; } | संख्या मान और समय संक्षेप (1 wk बनाम 1wk) के पहले स्पेस जोड़ने को दर्शाने वाला मान प्राप्त करता है या सेट करता है। |
| [DayLabel](../../aspose.tasks/projectdisplayoptions/daylabel/) { get; set; } | दिन लेबल कैसे प्रदर्शित होता है, इसे प्राप्त करता है या सेट करता है। |
| [HourLabel](../../aspose.tasks/projectdisplayoptions/hourlabel/) { get; set; } | घंटा लेबल कैसे प्रदर्शित होता है, इसे प्राप्त करता है या सेट करता है। |
| [MinuteLabel](../../aspose.tasks/projectdisplayoptions/minutelabel/) { get; set; } | मिनट लेबल कैसे प्रदर्शित होता है, इसे प्राप्त करता है या सेट करता है। |
| [MonthLabel](../../aspose.tasks/projectdisplayoptions/monthlabel/) { get; set; } | महीना लेबल कैसे प्रदर्शित होता है, इसे प्राप्त करता है या सेट करता है। |
| [ShowProjectSummaryTask](../../aspose.tasks/projectdisplayoptions/showprojectsummarytask/) { get; set; } | गैंट चार्ट व्यू के शीर्ष पर अपने स्वयं के समरी टास्क बार के साथ एक ही पंक्ति में पूरे प्रोजेक्ट की सारांश जानकारी प्रदर्शित करने को दर्शाने वाला मान प्राप्त करता है या सेट करता है। |
| [ShowTaskScheduleSuggestions](../../aspose.tasks/projectdisplayoptions/showtaskschedulesuggestions/) { get; set; } | जब प्रोजेक्ट मैन्युअली शेड्यूल किए गए टास्क के साथ संभावित शेड्यूलिंग कॉन्फ्लिक्ट पहचानता है, तो सुझाव दिखाने को दर्शाने वाला मान प्राप्त करता है या सेट करता है। यह विकल्प Project 2010 संस्करण और उसके बाद के संस्करणों के लिए उपलब्ध है। |
| [ShowTaskScheduleWarnings](../../aspose.tasks/projectdisplayoptions/showtaskschedulewarnings/) { get; set; } | प्रोजेक्ट द्वारा मैन्युअल रूप से निर्धारित कार्य में संभावित शेड्यूलिंग टकराव की पहचान होने पर चेतावनियाँ दिखाने के लिए मान प्राप्त करता है या सेट करता है। यह विकल्प प्रोजेक्ट 2010 संस्करण और बाद के संस्करणों के लिए उपलब्ध है। |
| [UnderlineHyperlinks](../../aspose.tasks/projectdisplayoptions/underlinehyperlinks/) { get; set; } | हाइपरलिंक को रेखांकित करने के लिए मान प्राप्त करता है या सेट करता है। |
| [WeekLabel](../../aspose.tasks/projectdisplayoptions/weeklabel/) { get; set; } | सप्ताह लेबल कैसे प्रदर्शित होता है, इसे प्राप्त करता है या सेट करता है। |
| [YearLabel](../../aspose.tasks/projectdisplayoptions/yearlabel/) { get; set; } | वर्ष लेबल कैसे प्रदर्शित होता है, इसे प्राप्त करता है या सेट करता है। |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


