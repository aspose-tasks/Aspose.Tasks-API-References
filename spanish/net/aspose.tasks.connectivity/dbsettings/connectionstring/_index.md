---
title: "DbSettings.ConnectionString"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad DbSettings. Obtiene o establece la cadena de conexión."
type: docs
weight: 10
url: /es/net/aspose.tasks.connectivity/dbsettings/connectionstring/
---
## DbSettings.ConnectionString property

Obtiene o establece la cadena de conexión.

```csharp
public string ConnectionString { get; set; }
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


