---
title: "क्लास TableTextStyle"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.TableTextStyle क्लास। एक दृश्य तालिका में टेक्स्ट शैली का प्रतिनिधित्व करता है।"
type: docs
weight: 3370
url: /hi/net/aspose.tasks.visualization/tabletextstyle/
---
## TableTextStyle class

दृश्य तालिका में टेक्स्ट शैली को दर्शाता है।

```csharp
public class TableTextStyle : TextStyle
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [TableTextStyle](tabletextstyle/#constructor)(int) | `TableTextStyle` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [TableTextStyle](tabletextstyle/#constructor_1)(int, FontDescriptor) | निर्दिष्ट फ़ॉन्ट के साथ `TableTextStyle` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [TableTextStyle](tabletextstyle/#constructor_2)(int, FontStyles) | डिफ़ॉल्ट फ़ॉन्ट सेटिंग्स और निर्दिष्ट फ़ॉन्ट स्टाइल के साथ `TableTextStyle` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [TableTextStyle](tabletextstyle/#constructor_3)(int, float, FontStyles) | निर्दिष्ट फ़ॉन्ट आकार और फ़ॉन्ट स्टाइल के साथ `TableTextStyle` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [BackgroundColor](../../aspose.tasks.visualization/textstyle/backgroundcolor/) { get; set; } | टेक्स्ट शैली का बैकग्राउंड रंग प्राप्त करता है या सेट करता है। [`Color`](../textstyle/color/). |
| [BackgroundPattern](../../aspose.tasks.visualization/textstyle/backgroundpattern/) { get; set; } | टेक्स्ट शैली का बैकग्राउंड पैटर्न प्राप्त करता है या सेट करता है। [`BackgroundPattern`](../textstyle/backgroundpattern/). |
| [Color](../../aspose.tasks.visualization/textstyle/color/) { get; set; } | टेक्स्ट का रंग प्राप्त करता है या सेट करता है। |
| [Field](../../aspose.tasks.visualization/tabletextstyle/field/) { get; set; } | उस फ़ील्ड को प्राप्त करता है या सेट करता है जिस पर शैली लागू होगी। [`Field`](./field/). |
| [Font](../../aspose.tasks.visualization/textstyle/font/) { get; set; } | टेक्स्ट शैली का फ़ॉन्ट प्राप्त करता है या सेट करता है। |
| override [ItemType](../../aspose.tasks.visualization/tabletextstyle/itemtype/) { get; } | [`TextItemType`](../textitemtype/) एन्‍युम का मान लौटाता है। |
| [RowUid](../../aspose.tasks.visualization/tabletextstyle/rowuid/) { get; } | एक पंक्ति का अद्वितीय आईडी प्राप्त करता है। यदि शैली सभी पंक्तियों पर लागू होनी है तो -1 लौटाएँ। |

## उदाहरण

प्रोजेक्ट में विभिन्न टेक्स्ट आइटम्स को स्टाइल करने के लिए उपयोग किए जाने वाले टेबल टेक्स्ट स्टाइल्स को कस्टमाइज़ करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.NewTasksAreManual, false);

var view = (GanttChartView)project.Views.ToList()[0];

// पहले टास्क नाम के टेक्स्ट स्टाइल को सेट करें
var style1 = new TableTextStyle(1);
// उस फ़ील्ड को सेट करें जिस पर स्टाइल लागू किया जाना है।
style1.Field = Field.TaskName;
// टेक्स्ट स्टाइल के <see cref="P:Aspose.Tasks.Visualization.TextStyle.Font" /> को सेट करें।
style1.Font = new FontDescriptor("Impact", 12F, FontStyles.Bold | FontStyles.Italic);
// टेक्स्ट स्टाइल फ़ॉन्ट का आकार पॉइंट्स में सेट करें।

// दूसरे टास्क अवधि के टेक्स्ट स्टाइल को सेट करें
var style2 = new TableTextStyle(2);
style2.Field = Field.TaskDurationText;
style2.Font = new FontDescriptor("Impact", 16F, FontStyles.Underline);

view.TableTextStyles.Add(style1);
view.TableTextStyles.Add(style2);

SimpleSaveOptions options = new MPPSaveOptions
{
    // एक फ़्लैग सेट करें जो दर्शाता है कि व्यू डेटा लिखा जाना चाहिए
    WriteViewData = true
};
project.Save(OutDir + "WorkWithTableTextStyle_out.mpp", options);
```

### संबंधित देखें

* class [TextStyle](../textstyle/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


