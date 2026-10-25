---
title: "Clase RiskPatternCollection"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.RiskAnalysis.RiskPatternCollection. Representa una colección que contiene las instancias de la clase RiskPattern."
type: docs
weight: 1940
url: /es/net/aspose.tasks.riskanalysis/riskpatterncollection/
---
## RiskPatternCollection class

Representa una colección que contiene las instancias de la clase [`RiskPattern`](../riskpattern/).

```csharp
public class RiskPatternCollection : ICollection<RiskPattern>, IDictionary<Task, RiskPattern>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.tasks.riskanalysis/riskpatterncollection/count/) { get; } | Obtiene el número de elementos contenidos en esta colección. |
| [IsReadOnly](../../aspose.tasks.riskanalysis/riskpatterncollection/isreadonly/) { get; } | Obtiene un valor que indica si esta colección es de solo lectura; de lo contrario, false. |
| [Item](../../aspose.tasks.riskanalysis/riskpatterncollection/item/) { get; } | Obtiene la instancia de la clase [`RiskPattern`](../riskpattern/) para la tarea especificada. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.tasks.riskanalysis/riskpatterncollection/add/)(RiskPattern) | Agrega una instancia de la clase [`RiskPattern`](../riskpattern/) a esta colección. |
| [Clear](../../aspose.tasks.riskanalysis/riskpatterncollection/clear/)() | Elimina todos los elementos de esta colección. |
| [Contains](../../aspose.tasks.riskanalysis/riskpatterncollection/contains/)(RiskPattern) | Devuelve true si el elemento especificado se encuentra en esta colección; de lo contrario, false. |
| [CopyTo](../../aspose.tasks.riskanalysis/riskpatterncollection/copyto/)(RiskPattern[], int) | Copia los elementos de esta colección al array especificado, comenzando en el índice de array especificado. |
| [GetEnumerator](../../aspose.tasks.riskanalysis/riskpatterncollection/getenumerator/)() | Devuelve un enumerador para esta colección. |
| [Remove](../../aspose.tasks.riskanalysis/riskpatterncollection/remove/)(RiskPattern) | Elimina la primera aparición de un objeto específico de esta colección. |

## Ejemplos

Muestra cómo trabajar con colecciones de patrones de riesgo.

```csharp
var settings = new RiskAnalysisSettings
{
    // Establece el número de iteraciones para la simulación Monte Carlo (el valor predeterminado es 100).
    IterationsCount = 200
};

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task1 = project.RootTask.Children.GetById(17);
var task2 = project.RootTask.Children.GetById(18);

// siempre que RiskPatternCollection no sea de solo lectura
Console.WriteLine("Is pattern collection read-only?: " + settings.Patterns.IsReadOnly);

// se pueden agregar nuevos patrones
var pattern1 = new RiskPattern(task1)
{
    Distribution = ProbabilityDistributionType.Normal,
    Optimistic = 60,
    Pessimistic = 140,
    ConfidenceLevel = ConfidenceLevel.CL75
};
var pattern2 = new RiskPattern(task2)
{
    Distribution = ProbabilityDistributionType.Normal,
    Optimistic = 70,
    Pessimistic = 130,
    ConfidenceLevel = ConfidenceLevel.CL75
};

settings.Patterns.Add(pattern1);
settings.Patterns.Add(pattern2);

// iterar sobre los patrones agregados
Console.WriteLine("Patterns count: " + settings.Patterns.Count);
foreach (var pattern in settings.Patterns)
{
    Console.WriteLine("Task: " + pattern.Task);
    Console.WriteLine("Distribution: " + pattern.Distribution);
    Console.WriteLine("Optimistic: " + pattern.Optimistic);
    Console.WriteLine("Pessimistic: " + pattern.Pessimistic);
    Console.WriteLine("Confidence Level: " + pattern.ConfidenceLevel);
    Console.WriteLine();
}

// editar el patrón en la colección usando acceso por índice
settings.Patterns[task1].Optimistic = 70;
settings.Patterns[task1].Pessimistic = 140;

// verificar los patrones después de las ediciones
Console.WriteLine("Print edited patterns: ");
foreach (var pattern in settings.Patterns)
{
    Console.WriteLine("Task: " + pattern.Task);
    Console.WriteLine("Distribution: " + pattern.Distribution);
    Console.WriteLine("Optimistic: " + pattern.Optimistic);
    Console.WriteLine("Pessimistic: " + pattern.Pessimistic);
    Console.WriteLine("Confidence Level: " + pattern.ConfidenceLevel);
    Console.WriteLine();
}

// podemos eliminar el patrón
Console.WriteLine("Removing the first pattern...");
settings.Patterns.Remove(pattern1);

// verificar que el patrón no esté en la colección
Console.WriteLine("Is collection contains the first pattern?: " + settings.Patterns.Contains(pattern1));

// se puede limpiar la colección de dos maneras

// copiar los patrones al arreglo y eliminarlos uno por uno
var patterns = new RiskPattern[settings.Patterns.Count];
settings.Patterns.CopyTo(patterns, 0);
foreach (var pattern in patterns)
{
    settings.Patterns.Remove(pattern);
}

// o se puede vaciar una colección de patrones completamente
settings.Patterns.Clear();
```

### Ver también

* class [RiskPattern](../riskpattern/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


