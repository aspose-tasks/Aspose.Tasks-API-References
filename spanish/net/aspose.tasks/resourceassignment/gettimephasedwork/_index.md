---
title: "ResourceAssignment.GetTimephasedWork"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ResourceAssignment. Obtiene la cantidad de trabajo faseado en el intervalo de fecha y hora especificado"
type: docs
weight: 730
url: /es/net/aspose.tasks/resourceassignment/gettimephasedwork/
---
## GetTimephasedWork(DateTime, DateTime, TimephasedDataType) {#gettimephasedwork_1}

Obtiene la cantidad de trabajo por fases de tiempo para el intervalo de fecha y hora especificado.

```csharp
public TimeSpan GetTimephasedWork(DateTime start, DateTime end, 
    TimephasedDataType timephasedDataType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inicio | DateTime | Inicio del intervalo de fecha y hora. |
| fin | DateTime | Fin del intervalo de fecha y hora. |
| timephasedDataType | TimephasedDataType | Tipo de los datos faseados en el tiempo a utilizar. |

## Ejemplos

Muestra cómo calcular el trabajo de la asignación para un intervalo de fecha y hora arbitrario.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var assignment = project.ResourceAssignments.GetByUid(2);

// Imprimir el trabajo de assignmen's para cada hora.
for (DateTime hour = assignment.Start; hour <= assignment.Finish; hour = hour.AddHours(1))
{
    var work = assignment.GetTimephasedWork(hour, hour.AddHours(1), TimephasedDataType.AssignmentWork);
    Console.WriteLine("{0} : {1:N2}", hour, work.TotalHours);
}
```

### Ver también

* enum [TimephasedDataType](../../timephaseddatatype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedWork(DateTime, DateTime) {#gettimephasedwork}

Obtiene la cantidad de trabajo por fases de tiempo para el intervalo de fecha y hora especificado.

```csharp
public TimeSpan GetTimephasedWork(DateTime start, DateTime end)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inicio | DateTime | Inicio del intervalo de fecha y hora. |
| fin | DateTime | Fin del intervalo de fecha y hora. |

### Ver también

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


