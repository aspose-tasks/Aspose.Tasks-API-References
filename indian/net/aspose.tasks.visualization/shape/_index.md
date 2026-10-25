---
title: "एनम Shape"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.Shape एनम। बार शैली की शुरुआत या अंत में एक मार्कर का आकार, जिसे व्यू डेटा को कुछ SaveFileFormat में सहेजते समय रेंडर किया जाता है।"
type: docs
weight: 3360
url: /hi/net/aspose.tasks.visualization/shape/
---
## Shape enumeration

बार शैली की शुरुआत या अंत में एक मार्कर का आकार, जब व्यू डेटा को कुछ [`SaveFileFormat`](../../aspose.tasks.saving/savefileformat/) में सहेजा जाता है।

```csharp
public enum Shape
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| None | `0` | None आकार दर्शाता है। |
| VerticalLine | `1` | Vertical लाइन आकार दर्शाता है। |
| Pentagon | `2` | Pentagon आकार दर्शाता है। |
| Triangle | `3` | Triangle आकार दर्शाता है। |
| LeftBracket | `4` | Left ब्रैकेट आकार दर्शाता है। |
| RightBracket | `5` | Right ब्रैकेट आकार दर्शाता है। |
| ArrowDown | `6` | ArrowDown आकार दर्शाता है। |
| LeftFade | `7` | Left फेड आकार दर्शाता है। |
| RightFade | `8` | Right फेड आकार दर्शाता है। |
| Diamond | `9` | Diamond आकार दर्शाता है। |
| Circle | `10` | Circle आकार दर्शाता है। |

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


