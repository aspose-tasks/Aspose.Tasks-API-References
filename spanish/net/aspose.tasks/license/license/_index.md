---
title: "License.License"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor de License. Inicializa una nueva instancia de la clase License"
type: docs
weight: 10
url: /es/net/aspose.tasks/license/license/
---
## License constructor

Inicializa una nueva instancia de la clase [`License`](../).

```csharp
public License()
```

## Ejemplos

En este ejemplo, se intentará encontrar un archivo de licencia llamado MyLicense.lic en la carpeta que contiene el componente, en la carpeta que contiene el ensamblado que llama, en la carpeta del ensamblado de entrada y luego en los recursos incrustados del ensamblado que llama.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

el archivo jar del componente:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

Muestra cómo aplicar una licencia de Aspose.Tasks.

```csharp
var license = new License();
license.SetLicense("Aspose.Tasks.lic");
```

### Ver también

* class [License](../)
* namespace [Aspose.Tasks](../../license/)
* assembly [Aspose.Tasks](../../../)


