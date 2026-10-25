---
title: "एनम TextItemType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.TextItemType एनम। टेक्स्ट शैली बदलने के लिए आइटम प्रकार"
type: docs
weight: 3410
url: /hi/net/aspose.tasks.visualization/textitemtype/
---
## TextItemType enumeration

टेक्स्ट शैली को बदलने के लिए आइटम प्रकार।

```csharp
public enum TextItemType
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| RowColumnTitles | `0` | पंक्ति और कॉलम शीर्षक। |
| CriticalTasks | `1` | महत्वपूर्ण कार्य। |
| NoncriticalTasks | `2` | गैर-आवश्यक कार्य। |
| MilestoneTasks | `3` | माइलस्टोन कार्य। |
| InactiveTasks | `4` | निष्क्रिय कार्य। |
| SummaryTasks | `5` | सारांश कार्य। |
| AssignmentRow | `6` | असाइनमेंट पंक्ति। |
| TopTimescaleTier | `7` | शीर्ष समय-सीमा स्तर। |
| BottomTimescaleTier | `8` | निचला समय-सीमा स्तर। |
| MiddleTimescaleTier | `9` | मध्य समय-सीमा स्तर। |
| Resources | `10` | संसाधन शीट। |
| OverallocatedResources | `11` | अधिक आवंटित संसाधन। |
| TaskFilterHighlight | `12` | कार्य फ़िल्टर हाइलाइट टेक्स्ट आइटम। |
| BarTextBottom | `13` | बार टेक्स्ट नीचे टेक्स्ट आइटम। |
| BarTextInside | `14` | बार टेक्स्ट अंदर टेक्स्ट आइटम। |
| BarTextLeft | `15` | बार टेक्स्ट बाएँ टेक्स्ट आइटम। |
| BarTextRight | `16` | बार टेक्स्ट दाएँ टेक्स्ट आइटम। |
| BarTextTop | `17` | बार टेक्स्ट ऊपर टेक्स्ट आइटम। |
| MarkedTasks | `18` | चिह्नित कार्य टेक्स्ट आइटम। |
| ProjectSummary | `19` | परियोजना सारांश कार्य टेक्स्ट आइटम। |
| ExternalTasks | `20` | बाहरी कार्य टेक्स्ट आइटम। |
| Allocated | `21` | आवंटित टेक्स्ट आइटम। |
| ChangedCells | `22` | बदले हुए कोशिकाएँ। |

## उदाहरण

टेक्स्ट आइटम प्रकारों के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.ResourceSheet
};

var style = new TextStyle(FontStyles.Italic | FontStyles.Bold)
{
    Color = Color.OrangeRed
};

style.ItemType = TextItemType.OverallocatedResources;

options.TextStyles = new List<TextStyle>
{
    style
};
project.Save(OutDir + "CustomizeTextStyle_out.pdf", options);
```

### संबंधित देखें

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


