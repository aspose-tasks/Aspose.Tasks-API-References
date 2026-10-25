---
title: "Enum BarShape"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.BarShape enum. बार आयत का आकार"
type: docs
weight: 2950
url: /hi/net/aspose.tasks.visualization/barshape/
---
## BarShape enumeration

बार आयत का आकार।

```csharp
public enum BarShape
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Full | `0` | पूर्ण आयत बार आकार को दर्शाता है। |
| HalfHeight | `1` | ऊपर संरेखित आधा-ऊँचाई आयत बार आकार को दर्शाता है। |
| HalfHeightBottom | `2` | नीचे संरेखित आधा-ऊँचाई आयत बार आकार को दर्शाता है। |
| Thin | `3` | केंद्र संरेखित रेखा आकार को दर्शाता है। |
| None | `4` | कोई बार आकार नहीं दर्शाता है। |
| Middle | `5` | केंद्र संरेखित रेखा आकार को दर्शाता है। |
| LineBottom | `6` | नीचे संरेखित रेखा आकार को दर्शाता है। |
| LineTop | `7` | ऊपर संरेखित रेखा आकार को दर्शाता है। |

## उदाहरण

कस्टम बार शैलियों का उपयोग कैसे करें दिखाता है।

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    BarStyles = new List<BarStyle>()
};

// माइलस्टोन टास्क के लिए एक बार शैली जोड़ें
var style = new BarStyle();
// बार शैली का <see cref=\"T:Aspose.Tasks.Visualization.BarItemType\" /> सेट करें
style.ItemType = BarItemType.Milestone;
// बार शैली का <see cref=\"T:System.Drawing.Color\" /> सेट करें।
style.BarColor = Color.Green;
// बार शैली का <see cref=\"P:Aspose.Tasks.Visualization.BarStyle.BarShape\" /> सेट करें
style.BarShape = BarShape.HalfHeight;
// बार की शुरुआत में <see cref="T:Aspose.Tasks.Visualization.Shape" /> सेट करें
style.StartShape = Shape.LeftBracket;
// बार की शुरुआत में आकार का <see cref="T:System.Drawing.Color" /> सेट करें
style.StartShapeColor = Color.Aqua;
// बार के अंत में <see cref="T:Aspose.Tasks.Visualization.Shape" /> सेट करें
style.EndShape = Shape.RightBracket;
// बार के अंत में आकार का <see cref="T:System.Drawing.Color" /> सेट करें
style.EndShapeColor = Color.Aquamarine;
// बार के दाएँ ओर रेंडर करने के लिए टेक्स्ट सेट करें।
style.TextStyle = new TextStyle();
style.TextStyle.BackgroundColor = Color.Black;

// एक सुविधा मौजूद है जो बार के टेक्स्ट को परिवर्तित करने की अनुमति देती है।
// चलो बार के लिए रेंडर करने हेतु टेक्स्ट प्राप्त करने के लिए कनवर्टर सेट करें।
style.LeftBarTextConverter = task =>
{
    if (!task.Get(Tsk.Name).StartsWith("T"))
    {
        task.Set(Tsk.Name, "T" + task.Get(Tsk.Name));
    }

    return task.Get(Tsk.Name);
};

options.BarStyles.Add(style);

// परियोजना सहेजें।
project.Save(OutDir + "WorkWithBarStyle_out.mpp", options);
```

### संबंधित देखें

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


