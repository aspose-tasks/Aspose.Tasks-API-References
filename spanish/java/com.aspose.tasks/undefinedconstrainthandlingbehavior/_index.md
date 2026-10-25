---
title: "UndefinedConstraintHandlingBehavior"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Especifica el comportamiento utilizado para manejar tareas con restricciones indefinidas."
type: docs
weight: 329
url: /es/java/com.aspose.tasks/undefinedconstrainthandlingbehavior/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class UndefinedConstraintHandlingBehavior extends System.Enum
```

Especifica el comportamiento utilizado para manejar tareas con restricciones indefinidas.
## Campos

| Campo | Descripción |
| --- | --- |
| [None](#None) | El comportamiento predeterminado al cargar desde el formato XER. |
| [SubstituteWithStartNoEarlierThan](#SubstituteWithStartNoEarlierThan) | Se añaden restricciones con tipo 'ConstraintType.StartNoEarlierThan' y fecha = Inicio para tareas con restricción 'Undefined'. |
### None {#None}
```
public static final int None
```


El comportamiento predeterminado al cargar desde el formato XER. No se realiza ninguna acción. El tipo de restricción de la tarea se establece en 'ConstraintType.Undefined'.

### SubstituteWithStartNoEarlierThan {#SubstituteWithStartNoEarlierThan}
```
public static final int SubstituteWithStartNoEarlierThan
```


Se añaden restricciones con tipo 'ConstraintType.StartNoEarlierThan' y fecha = Inicio para tareas con restricción 'Undefined'.

