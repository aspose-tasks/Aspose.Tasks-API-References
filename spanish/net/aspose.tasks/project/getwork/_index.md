---
title: "Project.GetWork"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método del proyecto. Obtiene un objeto Duration con el valor Double especificado y el formato de trabajo predeterminado"
type: docs
weight: 1130
url: /es/net/aspose.tasks/project/getwork/
---
## Project.GetWork method

Obtiene el objeto [`Duration`](../../duration/) con el valor Double especificado y el formato de trabajo predeterminado.

```csharp
public Duration GetWork(double val)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | Double | valor double especificado. |

### Valor devuelto

Objeto Duration.

## Observaciones

Este método debe usarse con cuidado porque devuelve duraciones diferentes según la configuración de Project.WorkFormat. Por ejemplo, GetWork(1.0) devolverá 1 hora cuando Project.WorkFormat sea TimeUnitType.Hour o 1 día si Project.WorkFormat es TimeUnitType.Day.

## Ejemplos

Muestra cómo obtener un trabajo con el formato de trabajo predeterminado.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

Console.WriteLine("Project's work format: " + project.Get(Prj.WorkFormat));

// crear un valor de trabajo con el formato de trabajo predeterminado del proyecto
var work = project.GetWork(2);
Console.WriteLine("Work: " + work.TimeSpan);
Console.WriteLine("Time unit: " + work.TimeUnit);
```

### Ver también

* struct [Duration](../../duration/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


