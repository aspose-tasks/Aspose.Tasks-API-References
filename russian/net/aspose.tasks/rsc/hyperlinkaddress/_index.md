---
title: "Rsc.HyperlinkAddress"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Адрес гиперссылки, связанной с ресурсом"
type: docs
weight: 330
url: /ru/net/aspose.tasks/rsc/hyperlinkaddress/
---
## Rsc.HyperlinkAddress field

Адрес гиперссылки, связанной с ресурсом.

```csharp
public static readonly Key<string, RscKey> HyperlinkAddress;
```

## Примечания

Полный адрес (Hyperlink Href в Microsoft Project) гиперссылки представляет собой конкатенацию HyperlinkAddress и HyperlinkSubAddress.

## Примеры

Показывает, как читать/записывать свойства гиперссылок ресурсов.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Hyperlink, "Click to visit our site");
resource.Set(Rsc.HyperlinkAddress, "https://products.aspose.com");
resource.Set(Rsc.HyperlinkSubAddress, "/total/net");

Console.WriteLine("Hyperlink: " + resource.Get(Rsc.Hyperlink));
Console.WriteLine("Hyperlink Address: " + resource.Get(Rsc.HyperlinkAddress));
Console.WriteLine("Hyperlink Sub Address: " + resource.Get(Rsc.HyperlinkSubAddress));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


