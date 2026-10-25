---
title: "Enum EarnedValueMethodType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.EarnedValueMethodType enum. Especifica el método utilizado para calcular el valor ganado"
type: docs
weight: 480
url: /es/net/aspose.tasks/earnedvaluemethodtype/
---
## EarnedValueMethodType enumeration

Especifica el método utilizado para calcular el valor ganado.

```csharp
public enum EarnedValueMethodType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Undefined | `-1` | El campo no estaba definido en el archivo de proyecto original. |
| PercentComplete | `0` | Porcentaje completado |
| PhysicalPercentComplete | `1` | Porcentaje físico completado |

## Observaciones

Al exportar a XML, los valores Undefined se eliminarán del XML resultante.

## Ejemplos

Muestra cómo especificar el método utilizado para calcular el valor ganado (EarnedValueMethodType.PercentComplete).

```csharp
var project = new Project(DataDir + "Project2.mpp");
// establecer el tipo de método de valor ganado a 'PercentComplete'
project.Set(Prj.DefaultTaskEVMethod, EarnedValueMethodType.PercentComplete);
// trabajar con el proyecto...
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


