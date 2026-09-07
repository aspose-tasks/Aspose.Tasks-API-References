---
title: "DbSettings.ProviderFactory"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "DbSettings-Eigenschaft. Gibt eine Instanz von DbProviderFactory zurück oder legt sie fest, die zum Verbinden mit der Datenbank verwendet wird. Wenn sowohl ProviderFactory als auch ProviderInvariantName festgelegt sind, hat ProviderFactory Vorrang. Der Standardwert ist null"
type: docs
weight: 30
url: /de/net/aspose.tasks.connectivity/dbsettings/providerfactory/
---
## DbSettings.ProviderFactory property

Gibt eine Instanz von DbProviderFactory zurück oder legt sie fest, die zum Verbinden mit der Datenbank verwendet wird. Wenn sowohl ProviderFactory als auch ProviderInvariantName festgelegt sind, hat ProviderFactory Vorrang. Der Standardwert ist null.

```csharp
public DbProviderFactory ProviderFactory { get; set; }
```

## Beispiele

Zeigt, wie man ein Projekt aus einer Primavera-Datenbank importiert.

```csharp
// Initialisiert eine neue Instanz der Klasse PrimaveraDbSettings mit Verbindungszeichenfolge und Projekt-ID.
var settings = new PrimaveraDbSettings(GetConnectionString(), 4502);
settings.ProviderFactory = SqliteFactory.Instance;

Console.WriteLine("Project UID to read: " + settings.ProjectId);

// liest das Projekt mit UID = 4502.
var project = new Project(settings);
Console.WriteLine(project.Uid);
Console.WriteLine(project.Name);
Console.WriteLine(project.PrimaveraProperties.ShortName);
```

### Siehe auch

* class [DbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../dbsettings/)
* assembly [Aspose.Tasks](../../../)


