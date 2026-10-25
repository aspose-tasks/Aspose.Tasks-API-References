---
title: "CopyToOptions.CopyToOptions"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor de CopyToOptions. Inicializa una nueva instancia de la clase CopyToOptions"
type: docs
weight: 10
url: /es/net/aspose.tasks/copytooptions/copytooptions/
---
## CopyToOptions constructor

Inicializa una nueva instancia de la clase [`CopyToOptions`](../).

```csharp
public CopyToOptions()
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


