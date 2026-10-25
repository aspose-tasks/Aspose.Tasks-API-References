---
title: "LoadOptions.Encoding"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad LoadOptions. Obtiene o establece la codificación que se usa para leer un proyecto de los formatos HTML, MPX, XER y Primavera XML. La codificación predeterminada es UTF8"
type: docs
weight: 30
url: /es/net/aspose.tasks/loadoptions/encoding/
---
## LoadOptions.Encoding property

Obtiene o establece la codificación que se usa para leer un proyecto desde formatos HTML, MPX, XER y Primavera XML. La codificación predeterminada es UTF8.

```csharp
public Encoding Encoding { get; set; }
```

## Ejemplos

Muestra cómo especificar la codificación al abrir un proyecto desde un archivo Primavera XER.

```csharp
LoadOptions lo = new LoadOptions();
lo.Encoding = Encoding.GetEncoding(1251);
lo.PrimaveraReadOptions = new PrimaveraReadOptions();
var project = new Project("encoding1251.xer", lo);
```

### Ver también

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


