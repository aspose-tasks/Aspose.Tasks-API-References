---
title: "TableTextStyle.TableTextStyle"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TableTextStyle कंस्ट्रक्टर। TableTextStyle वर्ग का नया उदाहरण प्रारंभ करता है।"
type: docs
weight: 10
url: /hi/net/aspose.tasks.visualization/tabletextstyle/tabletextstyle/
---
## TableTextStyle(int) {#constructor}

एक नए [`TableTextStyle`](../) वर्ग का उदाहरण प्रारंभ करता है।

```csharp
public TableTextStyle(int rowUid)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| rowUid | Int32 | एक निर्दिष्ट पंक्ति का अद्वितीय आईडी। |

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

* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, FontDescriptor) {#constructor_1}

निर्दिष्ट फ़ॉन्ट के साथ एक नए [`TableTextStyle`](../) वर्ग का उदाहरण प्रारंभ करता है।

```csharp
public TableTextStyle(int rowUid, FontDescriptor font)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| rowUid | Int32 | एक निर्दिष्ट पंक्ति का अद्वितीय आईडी। |
| font | FontDescriptor | एक फ़ॉन्ट जिस पर टेक्स्ट शैली आधारित है। |

### संबंधित देखें

* class [FontDescriptor](../../fontdescriptor/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, float, FontStyles) {#constructor_3}

निर्दिष्ट फ़ॉन्ट आकार और फ़ॉन्ट शैली के साथ एक नए [`TableTextStyle`](../) वर्ग का उदाहरण प्रारंभ करता है।

```csharp
public TableTextStyle(int rowUid, float fontSize, FontStyles fontStyle)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| rowUid | Int32 | एक निर्दिष्ट पंक्ति का अद्वितीय आईडी। |
| fontSize | Single | फ़ॉन्ट का आकार जिस पर टेक्स्ट शैली आधारित है। |
| fontStyle | FontStyles | फ़ॉन्ट की शैली जिस पर टेक्स्ट शैली आधारित है। |

### संबंधित देखें

* enum [FontStyles](../../fontstyles/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, FontStyles) {#constructor_2}

डिफ़ॉल्ट फ़ॉन्ट सेटिंग्स और निर्दिष्ट फ़ॉन्ट शैली के साथ एक नए [`TableTextStyle`](../) वर्ग का उदाहरण प्रारंभ करता है।

```csharp
public TableTextStyle(int rowUid, FontStyles fontStyle)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| rowUid | Int32 | एक निर्दिष्ट पंक्ति का अद्वितीय आईडी। |
| fontStyle | FontStyles | फ़ॉन्ट की शैली जिस पर टेक्स्ट शैली आधारित है। |

### संबंधित देखें

* enum [FontStyles](../../fontstyles/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)


