---
title: "TextStyle.TextStyle"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор TextStyle. Инициализирует новый экземпляр класса TextStyle с настройками по умолчанию"
type: docs
weight: 10
url: /ru/net/aspose.tasks.visualization/textstyle/textstyle/
---
## TextStyle() {#constructor}

Инициализирует новый экземпляр класса [`TextStyle`](../) с настройками по умолчанию.

```csharp
public TextStyle()
```

## Примеры

Показывает, как настраивать стили текста, которые используются для оформления различных текстовых элементов в проекте.

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

### См. также

* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(float, FontStyles) {#constructor_3}

Инициализирует новый экземпляр класса [`TextStyle`](../) с шрифтом по умолчанию и указанным размером и стилем шрифта.

```csharp
public TextStyle(float fontSize, FontStyles fontStyle)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fontSize | Single | Размер шрифта TextStyle. |
| fontStyle | FontStyles | Стиль шрифта TextStyle. |

### См. также

* enum [FontStyles](../../fontstyles/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(FontStyles) {#constructor_2}

Инициализирует новый экземпляр класса [`TextStyle`](../) с шрифтом по умолчанию и указанным стилем шрифта.

```csharp
public TextStyle(FontStyles fontStyle)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fontStyle | FontStyles | Стиль шрифта, применяемый к шрифту по умолчанию. |

### См. также

* enum [FontStyles](../../fontstyles/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(FontDescriptor) {#constructor_1}

Инициализирует новый экземпляр класса [`TextStyle`](../) с указанными настройками шрифта.

```csharp
public TextStyle(FontDescriptor font)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| font | FontDescriptor | Шрифт TextStyle. |

### См. также

* class [FontDescriptor](../../fontdescriptor/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)


