---
title: "क्लास GanttChartView"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.GanttChartView क्लास। GanttChart दृश्य का प्रतिनिधित्व करता है"
type: docs
weight: 710
url: /hi/net/aspose.tasks/ganttchartview/
---
## GanttChartView class

एक GanttChart दृश्य का प्रतिनिधित्व करता है।

```csharp
public class GanttChartView : View
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [GanttChartView](ganttchartview/)() | `GanttChartView` क्लास का नया उदाहरण आरंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [AutoFilters](../../aspose.tasks/ganttchartview/autofilters/) { get; } | Gantt Chart दृश्य के ऑटो फ़िल्टरों की सूची प्राप्त करता है। |
| [BarRounding](../../aspose.tasks/ganttchartview/barrounding/) { get; set; } | बारों को निकटतम दिन तक गोल करने का संकेत देने वाले मान को प्राप्त या सेट करता है। डिफ़ॉल्ट मान True है। |
| [BarSize](../../aspose.tasks/ganttchartview/barsize/) { get; set; } | Gantt Chart में Gantt बारों की ऊँचाई (पॉइंट्स में) को प्राप्त या सेट करता है। |
| [BarStyles](../../aspose.tasks/ganttchartview/barstyles/) { get; } | Gantt Chart दृश्य के पैरेंट (सामान्य) बार शैलियों की सूची प्राप्त करता है। [`GanttBarStyle`](../../aspose.tasks.visualization/ganttbarstyle/). |
| [BottomTimescaleTier](../../aspose.tasks/ganttchartview/bottomtimescaletier/) { get; set; } | व्यू के नीचे टाइमस्केल टियर की सेटिंग्स को प्राप्त करता है या सेट करता है। [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/) |
| [CustomBarStyles](../../aspose.tasks/ganttchartview/custombarstyles/) { get; } | Gantt Chart दृश्य के कस्टम टास्क-विशिष्ट बार शैलियों की सूची प्राप्त करता है। [`GanttBarStyle`](../../aspose.tasks.visualization/ganttbarstyle/). |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | एकल दृश्य में उपयोग किए जाने वाले फ़िल्टर को प्राप्त करता है या सेट करता है। |
| [Gridlines](../../aspose.tasks/ganttchartview/gridlines/) { get; set; } | Gantt Chart दृश्य की [`Gridlines`](./gridlines/) की सूची प्राप्त या सेट करता है। |
| [Group](../../aspose.tasks/view/group/) { get; set; } | एकल दृश्य का समूह प्राप्त करता है या सेट करता है। |
| [HideRollupBarsWhenSummaryExpanded](../../aspose.tasks/ganttchartview/hiderollupbarswhensummaryexpanded/) { get; set; } | समरी टास्क को विस्तारित करने पर रोलअप बारों को छिपाने का संकेत देने वाले मान को प्राप्त या सेट करता है। |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Microsoft Project द्वारा एकल दृश्य के लिए फ़िल्टर को हाइलाइट करने के लिए मान प्राप्त करता है या सेट करता है। |
| [MiddleTimescaleTier](../../aspose.tasks/ganttchartview/middletimescaletier/) { get; set; } | दृश्य की मध्य टाइमस्केल टियर की सेटिंग्स प्राप्त करता है या सेट करता है। [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/). |
| [Name](../../aspose.tasks/view/name/) { get; set; } | View ऑब्जेक्ट का नाम प्राप्त करता है या सेट करता है। |
| [NonWorkingTimeColor](../../aspose.tasks/ganttchartview/nonworkingtimecolor/) { get; set; } | नॉन-वर्किंग टाइम रंग को प्राप्त या सेट करता है। |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | `[`PageInfo`](../view/pageinfo/)` क्लास का एक उदाहरण प्राप्त करता है। यह mpp फ़ाइल फ़ॉर्मेट में मौजूद पेज सेटअप डेटा का प्रतिनिधित्व करता है। |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | View ऑब्जेक्ट का पैरेंट प्राप्त करता है। केवल‑पढ़ने योग्य [`Project`](../project/). |
| [ProgressLines](../../aspose.tasks/ganttchartview/progresslines/) { get; set; } | Gantt Chart दृश्य के लिए प्रोग्रेस लाइनों को प्राप्त या सेट करता है। [`ProgressLines`](./progresslines/). |
| [RollUpGanttBars](../../aspose.tasks/ganttchartview/rollupganttbars/) { get; set; } | Gantt Chart पर बारों को रोल अप करने का संकेत देने वाले मान को प्राप्त या सेट करता है। |
| [Screen](../../aspose.tasks/view/screen/) { get; } | एकल दृश्य के लिए स्क्रीन प्रकार प्राप्त करता है। केवल‑पढ़ने योग्य [`ViewScreen`](../viewscreen/). |
| [ShowBarSplits](../../aspose.tasks/ganttchartview/showbarsplits/) { get; set; } | Gantt Chart पर टास्क स्प्लिट्स को दिखाने का संकेत देने वाले मान को प्राप्त या सेट करता है। |
| [ShowDrawings](../../aspose.tasks/ganttchartview/showdrawings/) { get; set; } | Gantt Chart पर ड्रॉइंग्स को दिखाने का संकेत देने वाले मान को प्राप्त या सेट करता है। |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Microsoft Project द्वारा रिबन में View या Other Views ड्रॉप‑डाउन सूची में एकल दृश्य नाम दिखाने के लिए मान प्राप्त करता है या सेट करता है। |
| [Table](../../aspose.tasks/view/table/) { get; set; } | एकल दृश्य की तालिका प्राप्त करता है या सेट करता है। |
| [TableTextStyles](../../aspose.tasks/ganttchartview/tabletextstyles/) { get; } | Gantt Chart दृश्य के टेबल टेक्स्ट शैलियों की सूची प्राप्त करता है। [`TableTextStyle`](../../aspose.tasks.visualization/tabletextstyle/). |
| [TextStyles](../../aspose.tasks/ganttchartview/textstyles/) { get; set; } | Gantt Chart दृश्य की [`TextStyle`](../../aspose.tasks.visualization/textstyle/) की सूची प्राप्त या सेट करता है। |
| [TimescaleSizePercentage](../../aspose.tasks/ganttchartview/timescalesizepercentage/) { get; set; } |  |
| [TopTimescaleTier](../../aspose.tasks/ganttchartview/toptimescaletier/) { get; set; } | दृश्य की शीर्ष टाइमस्केल टियर की सेटिंग्स प्राप्त करता है या सेट करता है। [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/). |
| [Type](../../aspose.tasks/view/type/) { get; } | एकल दृश्य में आइटम के प्रकार को प्राप्त करता है, जैसे कार्य या संसाधन। केवल‑पढ़ने योग्य [`ItemType`](../itemtype/). |
| [Uid](../../aspose.tasks/view/uid/) { get; } | एक दृश्य का अद्वितीय पहचानकर्ता प्राप्त करता है। |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements/) { get; } | दृश्य में [`OleObject`](../oleobject/) की प्लेसमेंट और उपस्थिति को दर्शाने वाले ऑब्जेक्ट्स का संग्रह प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto/)(View) | वर्तमान इंस्टेंस की समान प्रकार के दूसरे ऑब्जेक्ट के साथ तुलना करता है और एक पूर्णांक लौटाता है जो दर्शाता है कि वर्तमान इंस्टेंस क्रम में पहले, बाद में, या उसी स्थिति में है या नहीं। |
| override [Equals](../../aspose.tasks/view/equals/)(object) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| override [GetHashCode](../../aspose.tasks/view/gethashcode/)() | `[`Resource`](../resource/)` क्लास के इंस्टेंस के लिए हैश कोड मान लौटाता है। |

## उदाहरण

टाइमस्केल टियर्स को संशोधित करने का तरीका दिखाता है।

```csharp
var project = new Project();

// Gantt Chart View को इनिट करें
var view = new GanttChartView
{
    TopTimescaleTier = new TimescaleTier(),
    MiddleTimescaleTier = new TimescaleTier(),
    BottomTimescaleTier = new TimescaleTier()
};

// टाइम स्केल काउंट सेट करें
view.TopTimescaleTier.Count = 2;
view.TopTimescaleTier.Unit = TimescaleUnit.Quarters;
view.TopTimescaleTier.Label = DateLabel.QuarterQQyy;
view.TopTimescaleTier.ShowTicks = false;

view.MiddleTimescaleTier.Count = 2;
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
view.MiddleTimescaleTier.ShowTicks = false;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayDdd;
view.BottomTimescaleTier.Count = 2;
view.BottomTimescaleTier.ShowTicks = false;

// प्रोजेक्ट में Gantt Chart View जोड़ें
project.Views.Add(view);

// प्रोजेक्ट में कुछ परीक्षण डेटा जोड़ें
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");
task1.Set(Tsk.Duration, task1.ParentProject.GetDuration(24, TimeUnitType.Hour));
task2.Set(Tsk.Duration, task1.ParentProject.GetDuration(40, TimeUnitType.Hour));

// 'Timescale.DefinedInView' विकल्प का उपयोग करके टाइमस्केल सेटिंग्स (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier) के आधार पर टाइमस्केल रेंडर करें।
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    StartDate = DateTime.Now.AddDays(-30),
    EndDate = DateTime.Now.AddDays(30)
};

project.Save(OutDir + "WorkWithTimescaleTier_out.pdf", pdfSaveOptions);
```

### संबंधित देखें

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


