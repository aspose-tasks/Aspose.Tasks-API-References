---
title: "CopyToOptions.CopyViewData"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad CopyToOptions. Obtiene o establece un valor que indica si se deben copiar los datos de vista al copiar los datos del proyecto. El valor predeterminado es true"
type: docs
weight: 20
url: /es/net/aspose.tasks/copytooptions/copyviewdata/
---
## CopyToOptions.CopyViewData property

Obtiene o establece un valor que indica si se deben copiar los datos de vista al copiar los datos del proyecto. El valor predeterminado es true.

```csharp
public bool CopyViewData { get; set; }
```

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

* class [CopyToOptions](../)
* namespace [Aspose.Tasks](../../copytooptions/)
* assembly [Aspose.Tasks](../../../)


