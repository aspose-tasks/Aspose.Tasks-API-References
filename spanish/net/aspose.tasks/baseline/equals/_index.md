---
title: "Baseline.Equals"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Baseline método. Devuelve un valor que indica si esta instancia es igual a un objeto especificado"
type: docs
weight: 80
url: /es/net/aspose.tasks/baseline/equals/
---
## Equals(object) {#equals_1}

Devuelve un valor que indica si esta instancia es igual a un objeto especificado.

```csharp
public override bool Equals(object obj)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | Objeto | el objeto especificado con el que comparar esta instancia. |

### Valor devuelto

devuelve true si esta instancia es igual al objeto especificado; de lo contrario, false.

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

* class [Baseline](../)
* namespace [Aspose.Tasks](../../baseline/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(Baseline) {#equals}

Devuelve un valor que indica si esta instancia es igual a un objeto especificado.

```csharp
public bool Equals(Baseline other)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| otro | Baseline | el objeto especificado con el que comparar esta instancia. |

### Valor devuelto

devuelve true si esta instancia es igual al objeto especificado; de lo contrario, false.

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

* class [Baseline](../)
* namespace [Aspose.Tasks](../../baseline/)
* assembly [Aspose.Tasks](../../../)


