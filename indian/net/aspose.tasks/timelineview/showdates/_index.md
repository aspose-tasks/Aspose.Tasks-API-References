---
title: "TimelineView.ShowDates"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TimelineView प्रॉपर्टी। यह मान प्राप्त करता है जो दर्शाता है कि तिथियों को दिखाना है या नहीं"
type: docs
weight: 40
url: /hi/net/aspose.tasks/timelineview/showdates/
---
## TimelineView.ShowDates property

तिथियों को दिखाने का संकेत देने वाला मान प्राप्त करता है।

```csharp
public bool ShowDates { get; }
```

## उदाहरण

&lt;see cref="Aspose.Tasks.TimelineView" /&gt; के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project();

// एक टाइमलाइन व्यू को प्रारंभ करें
var view = new TimelineView();

// टाइमलाइन व्यू पर तिथियों को फॉर्मेट करने का तरीका दर्शाने वाला मान सेट करें।
view.DateFormat = DateFormat.DateDddDd;
// एकाधिक पंक्तियों पर ओवरलैप्ड टास्क दिखाने का संकेत देने वाला मान सेट करें।
view.DisplayOverlapped = true;
// पैन और ज़ूम नियंत्रण दिखाने का संकेत देने वाला मान सेट करें।
view.ShowPanZoom = true;
// टाइमस्केल दिखाने का संकेत देने वाला मान सेट करें।
view.ShowTimescale = true;
// आज को दर्शाने वाली रेखा दिखाने का संकेत देने वाला मान सेट करें।
view.ShowToday = true;
// टाइमलाइन में टास्क दिखाने के लिए उपयोग की जाने वाली रेखाओं की संख्या दर्शाने वाला मान सेट करें।
view.TextLinesCount = 2;

// एकाधिक पंक्तियों पर ओवरलैप्ड टास्क दिखाने का संकेत देने वाला मान प्राप्त करता है।
Console.WriteLine("Show Dates: " + view.ShowDates);

// व्यू को प्रोजेक्ट में जोड़ें
project.Views.Add(view);

// प्रोजेक्ट में कुछ परीक्षण डेटा जोड़ें
var task1 = project.RootTask.Children.Add("Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 4, 29, 8, 0, 0));
task1.Set(Tsk.Duration, task1.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Start, new DateTime(2020, 4, 29, 8, 0, 0));
task2.Set(Tsk.Duration, task1.ParentProject.GetDuration(40, TimeUnitType.Hour));

project.Save(OutDir + "SetTimeScaleCount_out.pdf", SaveFileFormat.Pdf);
```

### संबंधित देखें

* class [TimelineView](../)
* namespace [Aspose.Tasks](../../timelineview/)
* assembly [Aspose.Tasks](../../../)


