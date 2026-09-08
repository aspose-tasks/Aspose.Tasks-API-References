---
title: "Clase CopyToOptions"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.CopyToOptions. Permite especificar opciones adicionales al copiar datos del proyecto"
type: docs
weight: 340
url: /es/net/aspose.tasks/copytooptions/
---
## CopyToOptions class

Permite especificar opciones adicionales al copiar datos del proyecto.

```csharp
public class CopyToOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [CopyToOptions](copytooptions/)() | Inicializa una nueva instancia de la clase `CopyToOptions`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CopyViewData](../../aspose.tasks/copytooptions/copyviewdata/) { get; set; } | Obtiene o establece un valor que indica si se deben copiar los datos de vista al copiar los datos del proyecto. El valor predeterminado es true. |

## Ejemplos

Muestra cómo usar las opciones de copia del proyecto.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", OutDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(OutDir + "ProjectCopying_out.mpp");

// omitir la copia de datos de vista al copiar datos comunes del proyecto.
var copyToOptions = new CopyToOptions();
copyToOptions.CopyViewData = false;
project.CopyTo(mppProject, copyToOptions);
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


