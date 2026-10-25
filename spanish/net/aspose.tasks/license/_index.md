---
title: "Clase License"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.License. Proporciona métodos para licenciar el componente"
type: docs
weight: 980
url: /es/net/aspose.tasks/license/
---
## License class

Proporciona métodos para licenciar el componente.

```csharp
public sealed class License
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [License](license/)() | Inicializa una nueva instancia de la clase `License`. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [SetLicense](../../aspose.tasks/license/setlicense/#setlicense)(Stream) | Licencia el componente. |
| [SetLicense](../../aspose.tasks/license/setlicense/#setlicense_1)(string) | Licencia el componente. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


