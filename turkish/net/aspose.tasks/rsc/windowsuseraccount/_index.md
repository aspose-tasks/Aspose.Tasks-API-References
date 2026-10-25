---
title: "Rsc.WindowsUserAccount"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir kaynakla ilişkili NT hesabı"
type: docs
weight: 680
url: /tr/net/aspose.tasks/rsc/windowsuseraccount/
---
## Rsc.WindowsUserAccount field

Bir kaynakla ilişkili NT hesabı.

```csharp
public static readonly Key<string, RscKey> WindowsUserAccount;
```

## Örnekler

Kaynağın meta özelliklerini nasıl ayarlayacağını gösterir.

```csharp
var project = new Project(DataDir + "Project.mpp");

// Kaynak ekle ve kaynak meta verilerini ayarla
var resource = project.Resources.Add("Rsc 1");
resource.Set(Rsc.EMailAddress, "1@gmail.com");
resource.Set(Rsc.WindowsUserAccount, "user_acc1");
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


