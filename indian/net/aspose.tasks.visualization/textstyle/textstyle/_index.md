---
title: "TextStyle.TextStyle"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TextStyle कंस्ट्रक्टर। डिफ़ॉल्ट सेटिंग्स के साथ TextStyle क्लास का नया इंस्टेंस इनिशियलाइज़ करता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks.visualization/textstyle/textstyle/
---
## TextStyle() {#constructor}

डिफ़ॉल्ट सेटिंग्स के साथ [`TextStyle`](../) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

```csharp
public TextStyle()
```

## उदाहरण

दिखाता है कि प्रोजेक्ट में विभिन्न टेक्स्ट आइटम्स को स्टाइल करने के लिए उपयोग किए जाने वाले टेक्स्ट स्टाइल्स को कैसे कस्टमाइज़ किया जाए।

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.ResourceSheet
};

var style = new TextStyle();
style.Color = Color.OrangeRed;
style.Font = new FontDescriptor(FontFamily.GenericMonospace.Name, 10F, FontStyles.Bold | FontStyles.Italic);
style.ItemType = TextItemType.OverallocatedResources;
style.BackgroundColor = Color.Aqua;
style.BackgroundPattern = BackgroundPattern.DarkDither;

options.TextStyles = new List<TextStyle>
{
    style
};
project.Save(OutDir + "CustomizeTextStyle_out.pdf", options);
```

### संबंधित देखें

* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(float, FontStyles) {#constructor_3}

डिफ़ॉल्ट फ़ॉन्ट और निर्दिष्ट फ़ॉन्ट आकार और शैली के साथ [`TextStyle`](../) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

```csharp
public TextStyle(float fontSize, FontStyles fontStyle)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fontSize | Single | TextStyle का फ़ॉन्ट आकार। |
| fontStyle | FontStyles | TextStyle का फ़ॉन्ट शैली। |

### संबंधित देखें

* enum [FontStyles](../../fontstyles/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(FontStyles) {#constructor_2}

डिफ़ॉल्ट फ़ॉन्ट और निर्दिष्ट फ़ॉन्ट शैली के साथ [`TextStyle`](../) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

```csharp
public TextStyle(FontStyles fontStyle)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fontStyle | FontStyles | डिफ़ॉल्ट फ़ॉन्ट पर लागू करने के लिए फ़ॉन्ट शैली। |

### संबंधित देखें

* enum [FontStyles](../../fontstyles/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(FontDescriptor) {#constructor_1}

निर्दिष्ट फ़ॉन्ट सेटिंग्स के साथ [`TextStyle`](../) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

```csharp
public TextStyle(FontDescriptor font)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| font | FontDescriptor | TextStyle का फ़ॉन्ट। |

### संबंधित देखें

* class [FontDescriptor](../../fontdescriptor/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)


