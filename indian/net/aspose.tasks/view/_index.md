---
title: "क्लास View"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.View क्लास। प्रोजेक्ट में एक व्यू का प्रतिनिधित्व करता है"
type: docs
weight: 2890
url: /hi/net/aspose.tasks/view/
---
## View class

Project में एक दृश्य दर्शाता है।

```csharp
public class View : IComparable<View>
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [View](view/#constructor)() | `View` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [View](view/#constructor_1)(ViewScreen) | `View` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | एकल दृश्य में उपयोग किए जाने वाले फ़िल्टर को प्राप्त करता है या सेट करता है। |
| [Group](../../aspose.tasks/view/group/) { get; set; } | एकल दृश्य का समूह प्राप्त करता है या सेट करता है। |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Microsoft Project द्वारा एकल दृश्य के लिए फ़िल्टर को हाइलाइट करने के लिए मान प्राप्त करता है या सेट करता है। |
| [Name](../../aspose.tasks/view/name/) { get; set; } | View ऑब्जेक्ट का नाम प्राप्त करता है या सेट करता है। |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | [`PageInfo`](./pageinfo/) क्लास का एक इंस्टेंस प्राप्त करता है। mpp फ़ाइल फ़ॉर्मेट में मौजूद पेज सेटअप डेटा का प्रतिनिधित्व करता है। |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | View ऑब्जेक्ट का पैरेंट प्राप्त करता है। केवल‑पढ़ने योग्य [`Project`](../project/). |
| [Screen](../../aspose.tasks/view/screen/) { get; } | एकल दृश्य के लिए स्क्रीन प्रकार प्राप्त करता है। केवल‑पढ़ने योग्य [`ViewScreen`](../viewscreen/). |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Microsoft Project द्वारा रिबन में View या Other Views ड्रॉप‑डाउन सूची में एकल दृश्य नाम दिखाने के लिए मान प्राप्त करता है या सेट करता है। |
| [Table](../../aspose.tasks/view/table/) { get; set; } | एकल दृश्य की तालिका प्राप्त करता है या सेट करता है। |
| [Type](../../aspose.tasks/view/type/) { get; } | एकल दृश्य में आइटम के प्रकार को प्राप्त करता है, जैसे कार्य या संसाधन। केवल‑पढ़ने योग्य [`ItemType`](../itemtype/). |
| [Uid](../../aspose.tasks/view/uid/) { get; } | एक दृश्य का अद्वितीय पहचानकर्ता प्राप्त करता है। |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements/) { get; } | दृश्य में [`OleObject`](../oleobject/) की प्लेसमेंट और उपस्थिति को दर्शाने वाले ऑब्जेक्ट्स का संग्रह प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto/)(View) | वर्तमान इंस्टेंस की समान प्रकार के दूसरे ऑब्जेक्ट के साथ तुलना करता है और एक पूर्णांक लौटाता है जो दर्शाता है कि वर्तमान इंस्टेंस क्रम में पहले, बाद में, या उसी स्थिति में है या नहीं। |
| override [Equals](../../aspose.tasks/view/equals/)(object) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| override [GetHashCode](../../aspose.tasks/view/gethashcode/)() | `[`Resource`](../resource/)` क्लास के इंस्टेंस के लिए हैश कोड मान लौटाता है। |
| [operator ==](../../aspose.tasks/view/op_equality/) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| [operator &gt;](../../aspose.tasks/view/op_greaterthan/) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट से बड़ा है या नहीं। |
| [operator &gt;=](../../aspose.tasks/view/op_greaterthanorequal/) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट से बड़ा या बराबर है या नहीं। |
| [operator !=](../../aspose.tasks/view/op_inequality/) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर नहीं है या नहीं। |
| [operator &lt;](../../aspose.tasks/view/op_lessthan/) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट से छोटा है या नहीं। |
| [operator &lt;=](../../aspose.tasks/view/op_lessthanorequal/) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट से छोटा या बराबर है या नहीं। |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


