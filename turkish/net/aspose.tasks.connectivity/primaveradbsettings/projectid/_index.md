---
title: "PrimaveraDbSettings.ProjectId"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PrimaveraDbSettings özelliği. Okunacak projenin kimliğini alır."
type: docs
weight: 20
url: /tr/net/aspose.tasks.connectivity/primaveradbsettings/projectid/
---
## PrimaveraDbSettings.ProjectId property

Okunacak projenin kimliğini alır.

```csharp
public int ProjectId { get; }
```

## Örnekler

Bir Primavera veritabanından projenin nasıl içe aktarılacağını gösterir.

```csharp
// Bağlantı dizesi ve proje kimliği ile PrimaveraDbSettings sınıfının yeni bir örneğini başlat
var settings = new PrimaveraDbSettings(GetConnectionString(), 4502);
settings.ProviderFactory = SqliteFactory.Instance;

Console.WriteLine("Project UID to read: " + settings.ProjectId);

// UID = 4502 ile projeyi okuyun
var project = new Project(settings);
Console.WriteLine(project.Uid);
Console.WriteLine(project.Name);
Console.WriteLine(project.PrimaveraProperties.ShortName);
```

### Ayrıca Bakınız

* class [PrimaveraDbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../primaveradbsettings/)
* assembly [Aspose.Tasks](../../../)


