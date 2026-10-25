---
title: "Resource.TimephasedData"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad de Resource. Obtiene o establece una instancia de la clase TimephasedDataCollection para este objeto"
type: docs
weight: 740
url: /es/net/aspose.tasks/resource/timephaseddata/
---
## Resource.TimephasedData property

Obtiene o establece una instancia de [`TimephasedDataCollection`](../../timephaseddatacollection/) para este objeto.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## Observaciones

Lectura soportada solo para formato XML.

## Ejemplos

Muestra cómo leer los datos temporales del recurso.

```csharp
resource.Set(Rsc.Work, resource.ParentProject.GetWork(2));

project.SetBaseline(BaselineType.Baseline);

// Iterar sobre los datos temporales del recurso 
foreach (var td in resource.TimephasedData)
{
    Console.WriteLine(td.Start);
    Console.WriteLine(td.Finish);
}
```

### Ver también

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


