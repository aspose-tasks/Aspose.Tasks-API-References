---
title: "क्लास ProgressLines"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.ProgressLines class. Gantt चार्ट दृश्य में प्रोग्रेस लाइनों का प्रतिनिधित्व करता है"
type: docs
weight: 3290
url: /hi/net/aspose.tasks.visualization/progresslines/
---
## ProgressLines class

गैंट चार्ट दृश्य में प्रोग्रेस लाइनों को दर्शाता है।

```csharp
public class ProgressLines
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [ProgressLines](progresslines/)() | डिफ़ॉल्ट कन्स्ट्रक्टर। |

## गुण

| नाम | विवरण |
| --- | --- |
| [BeginAtDate](../../aspose.tasks.visualization/progresslines/beginatdate/) { get; set; } | प्रोग्रेस लाइनों को प्रदर्शित करने की तिथि को प्राप्त करता है या सेट करता है। |
| [BeginAtProjectStart](../../aspose.tasks.visualization/progresslines/beginatprojectstart/) { get; set; } | प्रोजेक्ट शुरू होने की तिथि से प्रोग्रेस लाइनों को प्रदर्शित करने का संकेत देने वाले मान को प्राप्त करता है या सेट करता है। |
| [DateFormat](../../aspose.tasks.visualization/progresslines/dateformat/) { get; set; } | तिथि प्रारूप को प्राप्त करता है या सेट करता है ([`DateLabel`](../datelabel/)). |
| [DisplayAtCurrentDate](../../aspose.tasks.visualization/progresslines/displayatcurrentdate/) { get; set; } | वर्तमान तिथि पर प्रोग्रेस लाइन को प्रदर्शित करने का संकेत देने वाले मान को प्राप्त करता है या सेट करता है। |
| [DisplayAtRecurringIntervals](../../aspose.tasks.visualization/progresslines/displayatrecurringintervals/) { get; set; } | आवर्ती अंतराल पर प्रोग्रेस लाइन को प्रदर्शित करने का संकेत देने वाले मान को प्राप्त करता है या सेट करता है। |
| [DisplaySelected](../../aspose.tasks.visualization/progresslines/displayselected/) { get; set; } | चयनित तिथियों पर प्रोग्रेस लाइनों को प्रदर्शित करने का संकेत देने वाले मान को प्राप्त करता है या सेट करता है। |
| [Font](../../aspose.tasks.visualization/progresslines/font/) { get; set; } | प्रोग्रेस लाइन लेबल के लिए उपयोग किए जाने वाले फ़ॉन्ट को प्राप्त करता है या सेट करता है। |
| [IsBaselinePlan](../../aspose.tasks.visualization/progresslines/isbaselineplan/) { get; set; } | बेसलाइन योजना या वास्तविक के लिए प्रोग्रेस लाइनों को प्रदर्शित करने का संकेत देने वाले मान को प्राप्त करता है या सेट करता है। |
| [LineColor](../../aspose.tasks.visualization/progresslines/linecolor/) { get; set; } | वर्तमान प्रोग्रेस लाइन के लिए लाइन रंग को प्राप्त करता है या सेट करता है। |
| [LinePattern](../../aspose.tasks.visualization/progresslines/linepattern/) { get; set; } | वर्तमान प्रोग्रेस लाइन का लाइन पैटर्न प्राप्त करता है या सेट करता है। [`LinePattern`](./linepattern/). |
| [OtherLineColor](../../aspose.tasks.visualization/progresslines/otherlinecolor/) { get; set; } | अन्य प्रोग्रेस लाइन का रंग प्राप्त करता है या सेट करता है। |
| [OtherLinePattern](../../aspose.tasks.visualization/progresslines/otherlinepattern/) { get; set; } | अन्य प्रोग्रेस लाइन के लिए लाइन पैटर्न प्राप्त करता है या सेट करता है। |
| [OtherProgressPointColor](../../aspose.tasks.visualization/progresslines/otherprogresspointcolor/) { get; set; } | अन्य प्रोग्रेस पॉइंट का रंग प्राप्त करता है या सेट करता है। |
| [OtherProgressPointShape](../../aspose.tasks.visualization/progresslines/otherprogresspointshape/) { get; set; } | अन्य प्रोग्रेस लाइन के प्रोग्रेस पॉइंट आकार को प्राप्त करता है या सेट करता है। |
| [ProgressPointColor](../../aspose.tasks.visualization/progresslines/progresspointcolor/) { get; set; } | प्रोग्रेस पॉइंट का रंग प्राप्त करता है या सेट करता है। |
| [ProgressPointShape](../../aspose.tasks.visualization/progresslines/progresspointshape/) { get; set; } | प्रोग्रेस पॉइंट आकार को प्राप्त करता है या सेट करता है। [`GanttBarEndShape`](../ganttbarendshape/). |
| [RecurringInterval](../../aspose.tasks.visualization/progresslines/recurringinterval/) { get; set; } | आवर्ती अंतराल को प्राप्त करता है या सेट करता है। [`RecurringInterval`](./recurringinterval/). |
| [SelectedDates](../../aspose.tasks.visualization/progresslines/selecteddates/) { get; } | चयनित तिथियों की सूची प्राप्त करता है जिससे प्रगति रेखाएँ प्रदर्शित की जा सकें। |
| [ShowDate](../../aspose.tasks.visualization/progresslines/showdate/) { get; set; } | प्रत्येक प्रगति रेखा के लिए तिथि दिखाने का संकेत देने वाले मान को प्राप्त करता है या सेट करता है। |

## उदाहरण

दिखाता है कि प्रोग्रेस लाइनों के साथ कैसे काम किया जाए।

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// आइए प्रोग्रेस लाइन को परिभाषित करें
view.ProgressLines = new ProgressLines();
var progressLines = view.ProgressLines;

// प्रोग्रेस लाइनों को दिखाने की तिथि सेट करें। आइए प्रोजेक्ट की स्टेटस तिथि सेट करें।
progressLines.BeginAtDate = project.Get(Prj.StatusDate);
// एक मान सेट करें जो दर्शाता है कि प्रोजेक्ट की प्रारंभ तिथि से प्रोग्रेस लाइनों को दिखाना है या नहीं
progressLines.BeginAtProjectStart = true;
// तिथि फ़ॉर्मेट सेट करें (<see cref="T:Aspose.Tasks.Visualization.DateLabel" />)।
progressLines.DateFormat = DateLabel.DayDddd;
// एक मान सेट करें जो दर्शाता है कि वर्तमान तिथि पर प्रोग्रेस लाइन दिखानी है या नहीं।
progressLines.DisplayAtCurrentDate = true;
// एक मान सेट करें जो दर्शाता है कि आवर्ती अंतराल पर प्रोग्रेस लाइन दिखानी है या नहीं।
progressLines.DisplayAtRecurringIntervals = true;
// एक मान सेट करें जो दर्शाता है कि चयनित तिथियों पर प्रोग्रेस लाइनों को दिखाना है या नहीं
progressLines.DisplaySelected = true;
// एक मान सेट करें जो दर्शाता है कि बेसलाइन योजना या वास्तविक के लिए प्रोग्रेस लाइनों को दिखाना है या नहीं।
progressLines.IsBaselinePlan = false;
// प्रोग्रेस लाइन लेबल के लिए उपयोग किए जाने वाले फ़ॉन्ट को सेट करें।
progressLines.Font = new FontDescriptor("Arial", 10);
// वर्तमान प्रोग्रेस लाइन के लिए रेखा का रंग सेट करें।
progressLines.LineColor = Color.Aquamarine;
// वर्तमान प्रोग्रेस लाइन का रेखा पैटर्न सेट करें।
progressLines.LinePattern = LinePattern.Dashed;
// अन्य प्रोग्रेस लाइन का रंग सेट करें।
progressLines.OtherLineColor = Color.Azure;
// अन्य प्रोग्रेस लाइन के लिए रेखा पैटर्न सेट करें।
progressLines.OtherLinePattern = LinePattern.Dotted;
// अन्य प्रोग्रेस पॉइंट का रंग सेट करें।
progressLines.OtherProgressPointColor = Color.Red;
// अन्य प्रोग्रेस लाइन के प्रोग्रेस पॉइंट का आकार सेट करें।
progressLines.OtherProgressPointShape = GanttBarEndShape.Circle;
// प्रोग्रेस पॉइंट का रंग सेट करें।
progressLines.ProgressPointColor = Color.Orange;
// प्रोग्रेस पॉइंट का आकार सेट करें।
progressLines.ProgressPointShape = GanttBarEndShape.Diamond;
// आवर्ती अंतराल सेट करें।
progressLines.RecurringInterval = new RecurringInterval();
// आवर्ती अंतराल सेट करें।
progressLines.RecurringInterval.Interval = Interval.Daily;
// दैनिक दिन संख्या सेट करें
progressLines.RecurringInterval.DailyDayNumber = 1;
// प्रत्येक प्रोग्रेस लाइन के लिए तिथि दिखाने का संकेत देने वाला मान सेट करें।
progressLines.ShowDate = true;

// आइए प्रोग्रेस लाइनों की जाँच करें
Console.WriteLine("Begin At Date: " + progressLines.BeginAtDate);
Console.WriteLine("Begin At Project Start: " + progressLines.BeginAtProjectStart);
Console.WriteLine("Date Format: " + progressLines.DateFormat);
Console.WriteLine("Display At Current Date: " + progressLines.DisplayAtCurrentDate);
Console.WriteLine("Display At Recurring Intervals: " + progressLines.DisplayAtRecurringIntervals);
Console.WriteLine("Display Selected: " + progressLines.DisplaySelected);
Console.WriteLine("Font: " + progressLines.Font);
Console.WriteLine("Is Baseline Plan: " + progressLines.IsBaselinePlan);
Console.WriteLine("Line Color: " + progressLines.LineColor);
Console.WriteLine("Line Pattern: " + progressLines.LinePattern);
Console.WriteLine("Other Line Color: " + progressLines.OtherLineColor);
Console.WriteLine("Other Line Pattern: " + progressLines.OtherLinePattern);
Console.WriteLine("Other Progress Point Color: " + progressLines.OtherProgressPointColor);
Console.WriteLine("Other Progress Point Shape: " + progressLines.OtherProgressPointShape);
Console.WriteLine("Progress Point Color: " + progressLines.ProgressPointColor);
Console.WriteLine("Progress Point Shape: " + progressLines.ProgressPointShape);
Console.WriteLine("Recurring Interval: " + progressLines.RecurringInterval.Interval);
Console.WriteLine("Recurring Interval DailyDayNumber: " + progressLines.RecurringInterval.DailyDayNumber);
Console.WriteLine("Selected Dates: ");
foreach (var date in progressLines.SelectedDates)
{
    Console.WriteLine("Date: " + date);
}
Console.WriteLine("Show Date: " + progressLines.ShowDate);
Console.WriteLine();

project.Save(OutDir + "WorkWithProgressLines_out.mpp", SaveFileFormat.Mpp);
```

### संबंधित देखें

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


