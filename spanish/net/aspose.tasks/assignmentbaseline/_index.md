---
title: "Clase AssignmentBaseline"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.AssignmentBaseline. Representa la línea base de una asignación de recurso"
type: docs
weight: 50
url: /es/net/aspose.tasks/assignmentbaseline/
---
## AssignmentBaseline class

Representa la línea base de una asignación de recurso.

```csharp
public class AssignmentBaseline : Baseline, IComparable<AssignmentBaseline>, 
    IEquatable<AssignmentBaseline>
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [AssignmentBaseline](assignmentbaseline/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BaselineNumber](../../aspose.tasks/baseline/baselinenumber/) { get; set; } | Obtiene o establece el número único de un registro de datos de línea base. |
| [Bcwp](../../aspose.tasks/baseline/bcwp/) { get; set; } | Obtiene o establece el costo presupuestado del trabajo realizado por un recurso para un proyecto hasta la fecha. |
| [Bcws](../../aspose.tasks/baseline/bcws/) { get; set; } | Obtiene o establece el costo presupuestado de un trabajo programado para un recurso. |
| [Cost](../../aspose.tasks/baseline/cost/) { get; set; } | Obtiene o establece el costo proyectado de un recurso cuando se guarda la línea base. |
| [Finish](../../aspose.tasks/assignmentbaseline/finish/) { get; set; } | Obtiene o establece la fecha de finalización programada de la asignación de recurso cuando se guardó la línea base. La fecha de finalización de la asignación de recurso cuando se guardó esta línea base. |
| [Start](../../aspose.tasks/assignmentbaseline/start/) { get; set; } | Obtiene o establece la fecha de inicio programada de la asignación de recurso cuando se guardó la línea base. La fecha de inicio de la asignación de recurso cuando se guardó esta línea base. |
| [TimephasedData](../../aspose.tasks/assignmentbaseline/timephaseddata/) { get; set; } | Obtiene o establece la instancia de [`TimephasedDataCollection`](../timephaseddatacollection/) para este objeto. Los datos por fases de tiempo asociados con la línea base de la asignación de recurso. Devuelve la instancia de [`TimephasedDataCollection`](../timephaseddatacollection/) para este objeto. La colección de datos por fases de tiempo asociados con esta línea base. |
| [Work](../../aspose.tasks/baseline/work/) { get; set; } | Obtiene o establece el trabajo asignado a un recurso cuando se guarda la línea base. La cantidad de trabajo asignado a un recurso cuando se guardó la línea base. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [CompareTo](../../aspose.tasks/assignmentbaseline/compareto/#compareto)(AssignmentBaseline) | Implementación de la interfaz IComparable. Compara esta instancia con el objeto Baseline especificado. |
| [CompareTo](../../aspose.tasks/baseline/compareto/)(Baseline) | Implementación de la interfaz IComparable. Compara esta instancia con el objeto Baseline especificado. |
| [Equals](../../aspose.tasks/assignmentbaseline/equals/#equals)(AssignmentBaseline) | Devuelve un valor que indica si esta instancia es igual al objeto AssignmentBaseline especificado. |
| [Equals](../../aspose.tasks/baseline/equals/)(Baseline) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| override [Equals](../../aspose.tasks/assignmentbaseline/equals/#equals_2)(object) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| override [GetHashCode](../../aspose.tasks/assignmentbaseline/gethashcode/)() |  |

## Ejemplos

Muestra cómo trabajar con líneas base de asignaciones.

```csharp
var project = new Project(DataDir + "AssignmentBaseline2007.mpp");

// Las líneas base de asignación se establecen cuando se establece la línea base en todo el proyecto
project.SetBaseline(BaselineType.Baseline);

// leer información de la línea base de asignación
foreach (var assignment in project.ResourceAssignments)
{
    foreach (var baseline in assignment.Baselines)
    {
        Console.WriteLine("Baseline Start: " + baseline.Start);
        Console.WriteLine("Baseline Finish: " + baseline.Finish);
        Console.WriteLine("Baseline Number: " + baseline.BaselineNumber);
        Console.WriteLine("Bcwp: " + baseline.Bcwp);
        Console.WriteLine("Bcws: " + baseline.Bcws);
        Console.WriteLine("Cost: " + baseline.Cost);
        Console.WriteLine("Work: " + baseline.Work);
        if (baseline.TimephasedData != null)
        {
            foreach (var td in baseline.TimephasedData)
            {
                Console.WriteLine("TD Start: " + td.Start);
                Console.WriteLine("TD Finish: " + td.Finish);
                Console.WriteLine("TD Timephased Data Type: " + td.TimephasedDataType);
                Console.WriteLine();
            }
        }

        Console.WriteLine();
    }

    Console.WriteLine();
}

// verificar igualdad de línea base
var assn1 = project.ResourceAssignments.GetByUid(5);
var assn2 = project.ResourceAssignments.GetByUid(7);

var assignmentBaseline1 = assn1.Baselines.ToList()[0];
var assignmentBaseline2 = assn2.Baselines.ToList()[0];

// las líneas base pueden compararse usando sobrecargas del método 'Equals'
Console.WriteLine("Are baselines equal: " + assignmentBaseline1.Equals(assignmentBaseline2));

// o usando operaciones aritméticas sobrecargadas
Console.WriteLine("Is baseline 1 less than baseline 2: " + (assignmentBaseline1 < assignmentBaseline2));

// el código hash de la línea base se basa en el número de línea base
Console.WriteLine("Assignment baseline 1 hashcode: " + assignmentBaseline1.GetHashCode());
Console.WriteLine("Assignment baseline 2 hashcode: " + assignmentBaseline2.GetHashCode());
```

### Ver también

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


