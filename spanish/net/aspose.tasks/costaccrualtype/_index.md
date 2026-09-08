---
title: "Enum CostAccrualType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.CostAccrualType enum. Especifica el tipo de costo acumulado"
type: docs
weight: 350
url: /es/net/aspose.tasks/costaccrualtype/
---
## CostAccrualType enumeration

Especifica el tipo de costo acumulado.

```csharp
public enum CostAccrualType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Undefined | `-1` | Indica que un valor indefinido significa que el campo no estaba definido en el archivo de proyecto original. |
| Start | `0` | Indica el tipo de acumulación de costo Start. |
| Prorated | `1` | Indica el tipo de acumulación de costo Prorated. |
| End | `2` | Indica el tipo de acumulación de costo End. |
| Invalid | `3` | Indica el tipo de acumulación de costo Invalid. |

## Observaciones

Al exportar a XML, los valores Undefined se eliminarán del XML resultante.

## Ejemplos

Muestra cómo y cuándo se deben cobrar o acumular los costos estándar y de horas extra de los recursos (método de acumulación: Determina cuándo se incurre en el costo de un recurso y cuándo se cargan los costos reales a un proyecto. Puedes incurrir en costos al inicio [Start] o al final [End] de una tarea o prorratearlos [Prorated] durante la tarea.), al costo de una tarea (CostAccrualType.End).

```csharp
var project = new Project(DataDir + "Project2.mpp");
var resource = project.Resources.GetById(1);
// establecer tipo de acumulación de costo
// si seleccionas la opción End, los costos no se acumulan hasta que el trabajo restante sea cero.
resource.Set(Rsc.AccrueAt, CostAccrualType.End);
// trabajar con el proyecto...
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


