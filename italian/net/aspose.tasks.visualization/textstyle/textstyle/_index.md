---
title: "TextStyle.TextStyle"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore TextStyle. Inizializza una nuova istanza della classe TextStyle con impostazioni predefinite"
type: docs
weight: 10
url: /it/net/aspose.tasks.visualization/textstyle/textstyle/
---
## TextStyle() {#constructor}

Inizializza una nuova istanza della classe [`TextStyle`](../) con impostazioni predefinite.

```csharp
public TextStyle()
```

## Esempi

Mostra come personalizzare gli stili di testo che vengono usati per formattare diversi elementi di testo in un progetto.

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

### Vedi anche

* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(float, FontStyles) {#constructor_3}

Inizializza una nuova istanza della classe [`TextStyle`](../) con il carattere predefinito e la dimensione e lo stile del carattere specificati.

```csharp
public TextStyle(float fontSize, FontStyles fontStyle)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fontSize | Single | Dimensione del carattere di TextStyle. |
| fontStyle | FontStyles | Stile del carattere di TextStyle. |

### Vedi anche

* enum [FontStyles](../../fontstyles/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(FontStyles) {#constructor_2}

Inizializza una nuova istanza della classe [`TextStyle`](../) con il carattere predefinito e lo stile del carattere specificati.

```csharp
public TextStyle(FontStyles fontStyle)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fontStyle | FontStyles | Stile del carattere da applicare al carattere predefinito. |

### Vedi anche

* enum [FontStyles](../../fontstyles/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(FontDescriptor) {#constructor_1}

Inizializza una nuova istanza della classe [`TextStyle`](../) con le impostazioni del carattere specificate.

```csharp
public TextStyle(FontDescriptor font)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| font | FontDescriptor | Carattere di TextStyle. |

### Vedi anche

* class [FontDescriptor](../../fontdescriptor/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)


