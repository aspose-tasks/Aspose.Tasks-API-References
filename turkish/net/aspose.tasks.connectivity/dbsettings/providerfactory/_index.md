---
title: "DbSettings.ProviderFactory"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "DbSettings özelliği. DB'ye bağlanmak için kullanılan DbProviderFactory örneğini alır veya ayarlar. ProviderFactory ve ProviderInvariantName her ikisi de ayarlanmışsa ProviderFactory önceliğe sahiptir. Varsayılan değer null'dur."
type: docs
weight: 30
url: /tr/net/aspose.tasks.connectivity/dbsettings/providerfactory/
---
## DbSettings.ProviderFactory property

Veritabanına bağlanmak için kullanılan DbProviderFactory örneğini alır veya ayarlar. ProviderFactory ve ProviderInvariantName her ikisi de ayarlanmışsa, ProviderFactory önceliğe sahiptir. Varsayılan değer null'dur.

```csharp
public DbProviderFactory ProviderFactory { get; set; }
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

* class [DbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../dbsettings/)
* assembly [Aspose.Tasks](../../../)


