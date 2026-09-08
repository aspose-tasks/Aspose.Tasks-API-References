---
title: "Перечисление PrinterPaperSize"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.Visualization.PrinterPaperSize. Указывает размер бумаги, используемый для печати."
type: docs
weight: 3280
url: /ru/net/aspose.tasks.visualization/printerpapersize/
---
## PrinterPaperSize enumeration

Указывает размер бумаги, используемый для печати.

```csharp
public enum PrinterPaperSize
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Custom | `1` | Указывает, что размер бумаги задаётся пользователем. |
| PaperLetter | `1` | Указывает размер бумаги для принтера Envelope Letter (8.5 in. by 11 in.). |
| PaperLetterSmall | `2` | Указывает размер бумаги для принтера Small Letter (8.5 in. by 11 in.). |
| PaperTabloid | `3` | Указывает размер бумаги для принтера Tabloid (11 in. by 17 in.). |
| PaperLedger | `4` | Указывает размер бумаги для принтера Ledger (17 in. by 11 in.). |
| PaperLegal | `5` | Указывает размер бумаги для принтера Envelope legal (8.5 in. by 14 in.). |
| PaperStatement | `6` | Указывает размер бумаги для принтера Statement (5.5 in. by 8.5 in.). |
| PaperExecutive | `7` | Указывает размер бумаги для принтера Envelope executive (7.25 in. by 10.5 in.). |
| PaperA3 | `8` | Указывает размер бумаги для принтера A3 (297 mm by 420 mm). |
| PaperA4 | `9` | Указывает размер бумаги для принтера A4 (210 mm by 297 mm). |
| PaperA4Small | `10` | Указывает размер бумаги для принтера Small A4 (210 mm by 297 mm). |
| PaperA5 | `11` | Указывает размер бумаги для принтера A5 (148 mm by 210 mm). |
| PaperB4 | `12` | Указывает размер бумаги для принтера B4 (250 mm by 353 mm). |
| PaperB5 | `13` | Указывает размер бумаги для принтера B5 (176 mm by 250 mm). |
| PaperFolio | `14` | Указывает размер бумаги для принтера Folio (8.5 in. by 13 in.). |
| PaperQuarto | `15` | Указывает размер бумаги для принтера Quarto (215 mm by 275 mm). |
| PaperStandard10x14 | `16` | Указывает размер бумаги для принтера Standard (10 in. by 14 in.). |
| PaperStandard11x17 | `17` | Указывает размер бумаги для принтера Standard (11 in. by 17 in.). |
| PaperNote | `18` | Указывает размер бумаги для принтера Note (8.5 in. by 11 in.). |
| PaperEnvelope10 | `20` | Указывает размер бумаги для принтера Envelope10 (4.125 in. by 9.5 in.). |
| PaperCSheet | `24` | Указывает размер бумаги для принтера C paper (17 in. by 22 in.). |
| PaperDSheet | `25` | Указывает размер бумаги для принтера D paper (22 in. by 34 in.). |
| PaperESheet | `26` | Указывает размер бумаги для принтера E paper (34 in. by 44 in.). |
| PaperEnvelopeMonarch | `37` | Указывает размер бумаги для принтера Envelope Monarch (3.875 in. by 7.5 in.). |
| PaperStandard9x11 | `44` | Указывает размер бумаги для принтера Standard (9 in. by 11 in.). |
| PaperStandard10x11 | `45` | Указывает размер бумаги для принтера Standard (10 in. by 11 in.). |
| PaperStandard15x11 | `46` | Указывает стандартный размер бумаги для принтера (15 дюймов на 11 дюймов). |
| PaperA2 | `66` | Указывает размер бумаги A2 для принтера (420 мм на 594 мм). |

## Примеры

Показывает, как работать с информацией о странице в представлении MS Project.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// позволяет изменить представление по умолчанию
var info = project.DefaultView.PageInfo;

Console.WriteLine("Modify Page Info: " + info.Name);

// позволяет изменить поля
info.Margins.Left = 10d;
info.Margins.Top = 10d;
info.Margins.Right = 10d;
info.Margins.Bottom = 10d;

// давайте изменим настройки страницы
info.PageSettings.IsPortrait = true;
info.PageSettings.PaperSize = PrinterPaperSize.PaperA4;

// давайте изменим настройки представления страницы
// установите значение, указывающее, следует ли печатать заметки.
info.PageViewSettings.PrintNotes = true;

var header = new HeaderFooterInfo
{
    LeftText = "Left header text",
    CenteredText = "Centered header text",
    RightText = "Right header text"
};
var legend = new PageLegend
{
    LeftText =  "Left legend text",
    CenteredText = "Centered legend text",
    RightText = "Right legend text"
};
var footer = new HeaderFooterInfo
{
    LeftText = "Left footer text",
    CenteredText = "Centered footer text",
    RightText = "Right footer text"
};

info.Header = header;
info.Legend = legend;
info.Footer = footer;

// работать с проектом...
```

### См. также

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


