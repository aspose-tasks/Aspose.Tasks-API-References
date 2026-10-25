---
title: "Sınıf HeaderFooterInfo"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.HeaderFooterInfo sınıfı. Görünümlerin yazdırma ve render edilmesinde kullanılan başlık/altbilgi veya lejandın görsel içeriğini temsil eder."
type: docs
weight: 3130
url: /tr/net/aspose.tasks.visualization/headerfooterinfo/
---
## HeaderFooterInfo class

Görünümlerin yazdırma \ işlenmesi için kullanılan başlık, alt bilgi veya lejandın görsel içeriğini temsil eder.

```csharp
public class HeaderFooterInfo
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [HeaderFooterInfo](headerfooterinfo/)() | `HeaderFooterInfo` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CenteredImage](../../aspose.tasks.visualization/headerfooterinfo/centeredimage/) { get; set; } | Üst öğede görüntülenecek ortalanmış resmi alır veya ayarlar. |
| [CenteredImageSize](../../aspose.tasks.visualization/headerfooterinfo/centeredimagesize/) { get; set; } | Ortadaki görüntünün gösterilen boyutunu alır veya ayarlar. |
| [CenteredText](../../aspose.tasks.visualization/headerfooterinfo/centeredtext/) { get; set; } | Üst öğede görüntülenecek ortalanmış metni alır veya ayarlar. |
| [LeftImage](../../aspose.tasks.visualization/headerfooterinfo/leftimage/) { get; set; } | Üst öğede görüntülenecek sola hizalanmış resmi alır veya ayarlar. |
| [LeftImageSize](../../aspose.tasks.visualization/headerfooterinfo/leftimagesize/) { get; set; } | Sol resmin görüntülenen boyutunu alır veya ayarlar. |
| [LeftText](../../aspose.tasks.visualization/headerfooterinfo/lefttext/) { get; set; } | Üst öğede görüntülenecek sola hizalanmış metni alır veya ayarlar. |
| [RightImage](../../aspose.tasks.visualization/headerfooterinfo/rightimage/) { get; set; } | Üst öğede görüntülenecek sağa hizalanmış resmi alır veya ayarlar. |
| [RightImageSize](../../aspose.tasks.visualization/headerfooterinfo/rightimagesize/) { get; set; } | Sağ resmin görüntülenen boyutunu alır veya ayarlar. |
| [RightText](../../aspose.tasks.visualization/headerfooterinfo/righttext/) { get; set; } | Üst öğede görüntülenecek sağa hizalanmış metni alır veya ayarlar. |

## Örnekler

Sayfa üstbilgi/altbilgi bilgilerini nasıl okuyacağınızı gösterir.

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

### Ayrıca Bakınız

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


