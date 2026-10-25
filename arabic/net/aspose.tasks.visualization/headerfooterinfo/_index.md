---
title: "الفئة HeaderFooterInfo"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.Visualization.HeaderFooterInfo. تمثل المحتوى البصري للترويسة أو التذييل أو الأسطورة المستخدمة في طباعة وعرض المشاهد."
type: docs
weight: 3130
url: /ar/net/aspose.tasks.visualization/headerfooterinfo/
---
## HeaderFooterInfo class

يمثل المحتوى البصري للترويسة أو التذييل أو الأسطورة الذي يُستخدم للطباعة \ عرض المشاهد.

```csharp
public class HeaderFooterInfo
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [HeaderFooterInfo](headerfooterinfo/)() | ينشئ مثيلاً جديداً للفئة `HeaderFooterInfo`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CenteredImage](../../aspose.tasks.visualization/headerfooterinfo/centeredimage/) { get; set; } | يحصل أو يعيّن الصورة المركزية التي ستُعرض في العنصر الأب. |
| [CenteredImageSize](../../aspose.tasks.visualization/headerfooterinfo/centeredimagesize/) { get; set; } | يحصل أو يعيّن الحجم المعروض للصورة المركزية. |
| [CenteredText](../../aspose.tasks.visualization/headerfooterinfo/centeredtext/) { get; set; } | يحصل أو يعيّن النص المركزي لعرضه في العنصر الأب. |
| [LeftImage](../../aspose.tasks.visualization/headerfooterinfo/leftimage/) { get; set; } | يحصل أو يعيّن الصورة المحاذاة إلى اليسار التي تُعرض في العنصر الأب. |
| [LeftImageSize](../../aspose.tasks.visualization/headerfooterinfo/leftimagesize/) { get; set; } | يحصل أو يعيّن حجم الصورة اليسرى المعروض. |
| [LeftText](../../aspose.tasks.visualization/headerfooterinfo/lefttext/) { get; set; } | يحصل أو يعيّن النص المحاذى إلى اليسار لعرضه في العنصر الأب. |
| [RightImage](../../aspose.tasks.visualization/headerfooterinfo/rightimage/) { get; set; } | يحصل أو يعيّن الصورة المحاذاة إلى اليمين لتُعرض في العنصر الأب. |
| [RightImageSize](../../aspose.tasks.visualization/headerfooterinfo/rightimagesize/) { get; set; } | يحصل أو يعيّن حجم الصورة اليمنى المعروض. |
| [RightText](../../aspose.tasks.visualization/headerfooterinfo/righttext/) { get; set; } | يحصل أو يعيّن النص المحاذى إلى اليمين لعرضه في العنصر الأب. |

## الأمثلة

يعرض كيفية قراءة معلومات ترويسة/تذييل الصفحة.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");
var info = project.DefaultView.PageInfo;

Console.WriteLine("Header left text: {0} ", info.Header.LeftText);
Console.WriteLine("Header left image: {0} ", info.Header.LeftImage);
Console.WriteLine("Header left image size: {0} ", info.Header.LeftImageSize);
Console.WriteLine("Header center text: {0} ", info.Header.CenteredText);
Console.WriteLine("Header center image: {0} ", info.Header.CenteredImage);
Console.WriteLine("Header center image size: {0} ", info.Header.CenteredImageSize);
Console.WriteLine("Header right text: {0} ", info.Header.RightText);
Console.WriteLine("Header right image: {0} ", info.Header.RightImage);
Console.WriteLine("Header right image size: {0} ", info.Header.RightImageSize);
Console.WriteLine();
Console.WriteLine("Footer left text: {0} ", info.Footer.LeftText);
Console.WriteLine("Footer left image: {0} ", info.Footer.LeftImage);
Console.WriteLine("Footer left image size: {0} ", info.Footer.LeftImageSize);
Console.WriteLine("Footer center text: {0} ", info.Footer.CenteredText);
Console.WriteLine("Footer center image: {0} ", info.Footer.CenteredImage);
Console.WriteLine("Footer center size: {0} ", info.Footer.CenteredImageSize);
Console.WriteLine("Footer right text: {0} ", info.Footer.RightText);
Console.WriteLine("Footer right image: {0} ", info.Footer.RightImage);
Console.WriteLine("Footer right image size: {0} ", info.Footer.RightImageSize);
```

### انظر أيضًا

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


