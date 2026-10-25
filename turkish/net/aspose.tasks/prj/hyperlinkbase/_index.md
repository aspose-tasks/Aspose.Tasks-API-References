---
title: "Prj.HyperlinkBase"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Projelerin köprü temeli"
type: docs
weight: 380
url: /tr/net/aspose.tasks/prj/hyperlinkbase/
---
## Prj.HyperlinkBase field

Projenin köprü (hyperlink) temeli.

```csharp
public static readonly Key<string, PrjKey> HyperlinkBase;
```

## Örnekler

Prj.HyperlinkBase özelliğini okuma/yazma nasıl yapılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.HyperlinkBase, "www.aspose.com");

Console.WriteLine("Hyperlink Base: " + project.Get(Prj.HyperlinkBase));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


