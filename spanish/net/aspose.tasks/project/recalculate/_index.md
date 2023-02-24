---
title: Project.Recalculate
second_title: Referencia de Aspose.Tasks para la API de .NET
description: Project método. Reprograma todas las identificaciones de tareas del proyecto niveles de esquema fechas de inicio/finalización establece fechas tempranas/finales calcula espacios libres trabajo y campos de costos.
type: docs
weight: 1120
url: /es/net/aspose.tasks/project/recalculate/
---
## Recalculate() {#recalculate}

Reprograma todas las identificaciones de tareas del proyecto, niveles de esquema, fechas de inicio/finalización, establece fechas tempranas/finales, calcula espacios libres, trabajo y campos de costos.

```csharp
public void Recalculate()
```

### Ver también

* class [Project](../)
* espacio de nombres [Aspose.Tasks](../../project/)
* asamblea [Aspose.Tasks](../../../)

---

## Recalculate(bool) {#recalculate_1}

Reprograma todas las identificaciones de las tareas del proyecto, los niveles de esquema, las fechas de inicio/finalización, establece las fechas tempranas/finales, calcula los campos de trabajo y costos con validación opcional.

```csharp
public void Recalculate(bool validate)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| validate | Boolean | Si es verdadero, se realizará la validación del recálculo. Qué datos se validan: Por el momento, solo se implementa la validación básica de los intervalos de fechas de enlace de tareas y tareas. Intervalos de fechas de tareas (p. ej., inicio real - finalización real, inicio anticipado - finalización anticipada, etc. ), así como las fechas de los enlaces de tareas, se compararán con los criterios de fecha de que la fecha de inicio es menor o igual que la fecha de finalización. Si alguna de las condiciones descritas anteriormente falla, entonces[`RecalculationValidationException`](../../recalculationvalidationexception/)será lanzado. |

### Ver también

* class [Project](../)
* espacio de nombres [Aspose.Tasks](../../project/)
* asamblea [Aspose.Tasks](../../../)


