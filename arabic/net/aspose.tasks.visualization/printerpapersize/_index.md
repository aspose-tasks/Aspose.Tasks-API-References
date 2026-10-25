---
title: "التعداد PrinterPaperSize"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "التعداد Aspose.Tasks.Visualization.PrinterPaperSize. يحدد حجم الورق المستخدم للطباعة."
type: docs
weight: 3280
url: /ar/net/aspose.tasks.visualization/printerpapersize/
---
## PrinterPaperSize enumeration

يحدد حجم الورق المستخدم للطباعة.

```csharp
public enum PrinterPaperSize
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Custom | `1` | يشير إلى أن حجم الورق محدد من قبل المستخدم. |
| PaperLetter | `1` | يشير إلى حجم ورق الطابعة Envelope Letter (8.5 in. by 11 in.). |
| PaperLetterSmall | `2` | يشير إلى حجم ورق الطابعة Small Letter (8.5 in. by 11 in.). |
| PaperTabloid | `3` | يشير إلى حجم ورق الطابعة Tabloid (11 in. by 17 in.). |
| PaperLedger | `4` | يشير إلى حجم ورق الطابعة Ledger (17 in. by 11 in.). |
| PaperLegal | `5` | يشير إلى حجم ورق الطابعة Envelope legal (8.5 in. by 14 in.). |
| PaperStatement | `6` | يشير إلى حجم ورق الطابعة Statement (5.5 in. by 8.5 in.). |
| PaperExecutive | `7` | يشير إلى حجم ورق الطابعة Envelope executive (7.25 in. by 10.5 in.). |
| PaperA3 | `8` | يشير إلى حجم ورق الطابعة A3 (297 mm by 420 mm). |
| PaperA4 | `9` | يشير إلى حجم ورق الطابعة A4 (210 mm by 297 mm). |
| PaperA4Small | `10` | يشير إلى حجم ورق الطابعة Small A4 (210 mm by 297 mm). |
| PaperA5 | `11` | يشير إلى حجم ورق الطابعة A5 (148 mm by 210 mm). |
| PaperB4 | `12` | يشير إلى حجم ورق الطابعة B4 (250 mm by 353 mm). |
| PaperB5 | `13` | يشير إلى حجم ورق الطابعة B5 (176 mm by 250 mm). |
| PaperFolio | `14` | يشير إلى حجم ورق الطابعة Folio (8.5 in. by 13 in.). |
| PaperQuarto | `15` | يشير إلى حجم ورق الطابعة Quarto (215 mm by 275 mm). |
| PaperStandard10x14 | `16` | يشير إلى حجم ورق الطابعة Standard (10 in. by 14 in.). |
| PaperStandard11x17 | `17` | يشير إلى حجم ورق الطابعة Standard (11 in. by 17 in.). |
| PaperNote | `18` | يشير إلى حجم ورق الطابعة Note (8.5 in. by 11 in.). |
| PaperEnvelope10 | `20` | يشير إلى حجم ورق الطابعة Envelope10 (4.125 in. by 9.5 in.). |
| PaperCSheet | `24` | يشير إلى حجم ورق الطابعة C paper (17 in. by 22 in.). |
| PaperDSheet | `25` | يشير إلى حجم ورق الطابعة D paper (22 in. by 34 in.). |
| PaperESheet | `26` | يشير إلى حجم ورق الطابعة E paper (34 in. by 44 in.). |
| PaperEnvelopeMonarch | `37` | يشير إلى حجم ورق الطابعة Envelope Monarch (3.875 in. by 7.5 in.). |
| PaperStandard9x11 | `44` | يشير إلى حجم ورق الطابعة Standard (9 in. by 11 in.). |
| PaperStandard10x11 | `45` | يشير إلى حجم ورق الطابعة Standard (10 in. by 11 in.). |
| PaperStandard15x11 | `46` | يشير إلى حجم ورق الطابعة القياسي (15 بوصة × 11 بوصة). |
| PaperA2 | `66` | يشير إلى حجم ورق الطابعة A2 (420 مم × 594 مم). |

## الأمثلة

يعرض كيفية العمل مع معلومات الصفحة في عرض MS Project.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// دعنا نعدّل العرض الافتراضي.
var info = project.DefaultView.PageInfo;

Console.WriteLine("Modify Page Info: " + info.Name);

// دعنا نعدّل الهوامش.
info.Margins.Left = 10d;
info.Margins.Top = 10d;
info.Margins.Right = 10d;
info.Margins.Bottom = 10d;

// دعنا نُعدّل إعدادات الصفحة
info.PageSettings.IsPortrait = true;
info.PageSettings.PaperSize = PrinterPaperSize.PaperA4;

// دعنا نُعدّل إعدادات عرض الصفحة
// عيّن قيمة تشير إلى ما إذا كان يجب طباعة الملاحظات.
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

// العمل مع المشروع...
```

### انظر أيضًا

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


