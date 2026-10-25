---
title: "Enum BaselineType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enum Aspose.Tasks.BaselineType. Especifica el tipo de línea base usado para calcular los valores de variación."
type: docs
weight: 130
url: /es/net/aspose.tasks/baselinetype/
---
## BaselineType enumeration

Especifica el tipo de línea base utilizado para calcular los valores de variación.

```csharp
public enum BaselineType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Undefined | `-1` | Indica que el campo no estaba definido en el archivo de proyecto original. |
| Baseline | `0` | Indica el tipo de línea base. |
| Baseline1 | `1` | Indica el tipo de Baseline1. |
| Baseline2 | `2` | Indica el tipo de Baseline2. |
| Baseline3 | `3` | Indica el tipo de Baseline3. |
| Baseline4 | `4` | Indica el tipo de Baseline4. |
| Baseline5 | `5` | Indica el tipo de Baseline5. |
| Baseline6 | `6` | Indica el tipo de Baseline6. |
| Baseline7 | `7` | Indica el tipo de Baseline7. |
| Baseline8 | `8` | Indica el tipo de Baseline8. |
| Baseline9 | `9` | Indica el tipo de Baseline9. |
| Baseline10 | `10` | Indica el tipo de Baseline10. |

## Observaciones

Al exportar a XML, los valores Undefined se eliminarán del XML resultante.

## Ejemplos

Muestra cómo establecer la línea base para el proyecto (BaselineType.Baseline).

```csharp
var project = new Project(DataDir + "Project2.mpp");
// Guarda los campos de línea base en la línea base especificada para todo el proyecto.
project.SetBaseline(BaselineType.Baseline);
// Trabaja con las líneas base del proyecto...
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


