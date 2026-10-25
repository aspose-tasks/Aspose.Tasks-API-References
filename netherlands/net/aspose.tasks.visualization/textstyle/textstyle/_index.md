---
title: "TextStyle.TextStyle"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TextStyle-constructeur. Initialiseert een nieuw exemplaar van de TextStyle-klasse met standaardinstellingen"
type: docs
weight: 10
url: /nl/net/aspose.tasks.visualization/textstyle/textstyle/
---
## TextStyle() {#constructor}

Initialiseert een nieuw exemplaar van de [`TextStyle`](../)-klasse met standaardinstellingen.

```csharp
public TextStyle()
```

## Voorbeelden

Toont hoe tekststijlen aan te passen die worden gebruikt om verschillende tekstitems in een project op te maken.

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

### Zie ook

* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(float, FontStyles) {#constructor_3}

Initialiseert een nieuw exemplaar van de [`TextStyle`](../)-klasse met het standaardlettertype en de opgegeven lettergrootte en stijl.

```csharp
public TextStyle(float fontSize, FontStyles fontStyle)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fontSize | Single | Grootte van het lettertype van TextStyle. |
| fontStyle | FontStyles | Stijl van het lettertype van TextStyle. |

### Zie ook

* enum [FontStyles](../../fontstyles/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(FontStyles) {#constructor_2}

Initialiseert een nieuw exemplaar van de [`TextStyle`](../)-klasse met het standaardlettertype en de opgegeven letterstijl.

```csharp
public TextStyle(FontStyles fontStyle)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fontStyle | FontStyles | Lettertype-stijl die op het standaardlettertype moet worden toegepast. |

### Zie ook

* enum [FontStyles](../../fontstyles/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(FontDescriptor) {#constructor_1}

Initialiseert een nieuw exemplaar van de [`TextStyle`](../)-klasse met de opgegeven lettertype-instellingen.

```csharp
public TextStyle(FontDescriptor font)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| font | FontDescriptor | Lettertype van de TextStyle. |

### Zie ook

* class [FontDescriptor](../../fontdescriptor/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)


