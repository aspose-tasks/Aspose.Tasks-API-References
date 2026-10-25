---
title: "ProgressLines.OtherProgressPointColor"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ProgressLines प्रॉपर्टी। अन्य प्रोग्रेस पॉइंट का रंग प्राप्त करता है या सेट करता है।"
type: docs
weight: 140
url: /hi/net/aspose.tasks.visualization/progresslines/otherprogresspointcolor/
---
## ProgressLines.OtherProgressPointColor property

अन्य प्रोग्रेस पॉइंट का रंग प्राप्त करता है या सेट करता है।

```csharp
public Color OtherProgressPointColor { get; set; }
```

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

* class [ProgressLines](../)
* namespace [Aspose.Tasks.Visualization](../../progresslines/)
* assembly [Aspose.Tasks](../../../)


