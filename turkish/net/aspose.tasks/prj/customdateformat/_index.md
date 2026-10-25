---
title: "Prj.CustomDateFormat"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Proje görünümü özel tarih biçimi. DateFormat özelliği Custom olarak ayarlandığında tarihleri biçimlendirmek için kullanılır."
type: docs
weight: 200
url: /tr/net/aspose.tasks/prj/customdateformat/
---
## Prj.CustomDateFormat field

Proje görünümü özel tarih biçimi. [`DateFormat`](../dateformat/) özelliği Custom olarak ayarlandığında tarihleri biçimlendirmek için kullanılır.

```csharp
public static readonly Key<string, PrjKey> CustomDateFormat;
```

## Örnekler

Prj.CustomDateFormat özelliğini okuma/yazma nasıl yapılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.CustomDateFormat, "dd MMMM yyyy H:mm");

Console.WriteLine("Custom Date Format: " + project.Get(Prj.CustomDateFormat));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


