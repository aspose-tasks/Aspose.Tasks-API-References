---
title: "Enumeración UndefinedConstraintHandlingBehavior"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enumeración Aspose.Tasks.UndefinedConstraintHandlingBehavior. Especifica el comportamiento utilizado para manejar tareas con restricciones indefinidas."
type: docs
weight: 2630
url: /es/net/aspose.tasks/undefinedconstrainthandlingbehavior/
---
## UndefinedConstraintHandlingBehavior enumeration

Especifica el comportamiento utilizado para manejar tareas con restricciones indefinidas.

```csharp
public enum UndefinedConstraintHandlingBehavior
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | El comportamiento predeterminado para cargar desde el formato XER. No se realiza ninguna acción. El tipo de restricción de tarea se establece en 'ConstraintType.Undefined'. |
| SubstituteWithStartNoEarlierThan | `1` | Se añaden restricciones con tipo 'ConstraintType.StartNoEarlierThan' y fecha = Inicio para tareas con restricción 'Undefined'. |

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


