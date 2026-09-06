---
title: "TextStyle.TextStyle"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur TextStyle. Initialise une nouvelle instance de la classe TextStyle avec les paramètres par défaut"
type: docs
weight: 10
url: /fr/net/aspose.tasks.visualization/textstyle/textstyle/
---
## TextStyle() {#constructor}

Initialise une nouvelle instance de la classe [`TextStyle`](../) avec les paramètres par défaut.

```csharp
public TextStyle()
```

## Exemples

Montre comment personnaliser les styles de texte qui sont utilisés pour styliser différents éléments de texte dans un projet.

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

### Voir aussi

* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(float, FontStyles) {#constructor_3}

Initialise une nouvelle instance de la classe [`TextStyle`](../) avec la police par défaut et la taille et le style de police spécifiés.

```csharp
public TextStyle(float fontSize, FontStyles fontStyle)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fontSize | Single | Taille de la police du TextStyle. |
| fontStyle | FontStyles | Style de la police du TextStyle. |

### Voir aussi

* enum [FontStyles](../../fontstyles/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(FontStyles) {#constructor_2}

Initialise une nouvelle instance de la classe [`TextStyle`](../) avec la police par défaut et le style de police spécifié.

```csharp
public TextStyle(FontStyles fontStyle)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fontStyle | FontStyles | Style de police à appliquer à la police par défaut. |

### Voir aussi

* enum [FontStyles](../../fontstyles/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(FontDescriptor) {#constructor_1}

Initialise une nouvelle instance de la classe [`TextStyle`](../) avec les paramètres de police spécifiés.

```csharp
public TextStyle(FontDescriptor font)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| font | FontDescriptor | Police du TextStyle. |

### Voir aussi

* class [FontDescriptor](../../fontdescriptor/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)


