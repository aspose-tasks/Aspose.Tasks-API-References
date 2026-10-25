---
title: "TableTextStyle.ItemType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TableTextStyle प्रॉपर्टी। TextItemType एनम का मान लौटाता है।"
type: docs
weight: 30
url: /hi/net/aspose.tasks.visualization/tabletextstyle/itemtype/
---
## TableTextStyle.ItemType property

एक [`TextItemType`](../../textitemtype/) एनम का मान लौटाता है।

```csharp
public override TextItemType ItemType { get; }
```

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

* enum [TextItemType](../../textitemtype/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)


