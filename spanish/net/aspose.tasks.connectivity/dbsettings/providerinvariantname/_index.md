---
title: "DbSettings.ProviderInvariantName"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad DbSettings. Obtiene o establece el nombre invariante del proveedor que se usa para obtener una instancia de la clase DbProviderFactory. El valor predeterminado es SqlClient."
type: docs
weight: 40
url: /es/net/aspose.tasks.connectivity/dbsettings/providerinvariantname/
---
## DbSettings.ProviderInvariantName property

Obtiene o establece el nombre invariante del proveedor que se usa para obtener una instancia de la clase DbProviderFactory. El valor predeterminado es SqlClient.

```csharp
public string ProviderInvariantName { get; set; }
```

## Ejemplos

Muestra cómo leer un proyecto desde un archivo XML de Primavera con múltiples proyectos usando un nombre de proveedor.

```csharp
var connectionString = "Data Source=" + DataDir + "\\PPMDBSQLite.db";

// Crear configuraciones de DB de Primavera usando la cadena de conexión y el ID del proyecto
var settings = new PrimaveraDbSettings(connectionString, 4502);
settings.ProviderInvariantName = "System.Data.SQLite";

Console.WriteLine("Connection String: " + settings.ConnectionString);
Console.WriteLine("Provider Name: " + settings.ProviderInvariantName);

var project = new Project(settings);
project.Save(OutDir + "SupportForSQLiteDatabase_out.mpp", SaveFileFormat.Mpp);
```

### Ver también

* class [DbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../dbsettings/)
* assembly [Aspose.Tasks](../../../)


