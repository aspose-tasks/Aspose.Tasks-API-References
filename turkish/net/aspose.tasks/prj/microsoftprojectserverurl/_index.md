---
title: "Prj.MicrosoftProjectServerURL"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Bir projenin Project Server kullanıcısı tarafından mı yoksa NT kullanıcısı tarafından mı oluşturulduğunu belirler"
type: docs
weight: 460
url: /tr/net/aspose.tasks/prj/microsoftprojectserverurl/
---
## Prj.MicrosoftProjectServerURL field

Bir projenin NT kullanıcısı yerine Project Server kullanıcısı tarafından oluşturulup oluşturulmadığını belirler.

```csharp
public static readonly Key<NullableBool, PrjKey> MicrosoftProjectServerURL;
```

## Örnekler

Prj.MicrosoftProjectServerURL özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.MicrosoftProjectServerURL, true);

Console.WriteLine("Microsoft Project Server U R L: " + project.Get(Prj.MicrosoftProjectServerURL));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


