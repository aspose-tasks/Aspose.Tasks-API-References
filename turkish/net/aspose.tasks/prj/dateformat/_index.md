---
title: "Prj.DateFormat"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Proje görünümü tarih biçimi"
type: docs
weight: 210
url: /tr/net/aspose.tasks/prj/dateformat/
---
## Prj.DateFormat field

Proje görünümü tarih biçimi.

```csharp
public static readonly Key<DateFormat, PrjKey> DateFormat;
```

## Örnekler

Prj.DateFormat özelliğini okuma/yazma nasıl yapılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.DateFormat, DateFormat.DateDd);

Console.WriteLine("Date Format: " + project.Get(Prj.DateFormat));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [DateFormat](../../dateformat/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


