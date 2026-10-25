---
title: "Clase GraphicalIndicatorCriteria"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.GraphicalIndicatorCriteria. Representa un criterio de indicador gráfico asociado a un atributo extendido"
type: docs
weight: 730
url: /es/net/aspose.tasks/graphicalindicatorcriteria/
---
## GraphicalIndicatorCriteria class

Representa un criterio de indicador gráfico asociado a un atributo extendido.

```csharp
public sealed class GraphicalIndicatorCriteria
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [GraphicalIndicatorCriteria](graphicalindicatorcriteria/#constructor)(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue) | Inicializa una nueva instancia del tipo `GraphicalIndicatorCriteria`. |
| [GraphicalIndicatorCriteria](graphicalindicatorcriteria/#constructor_1)(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue, GraphicalIndicatorCriteriaValue) | Inicializa una nueva instancia del tipo `GraphicalIndicatorCriteria`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ImageIndex](../../aspose.tasks/graphicalindicatorcriteria/imageindex/) { get; } | Obtiene el índice de la imagen a mostrar cuando el campo cumple los criterios. |
| [RowType](../../aspose.tasks/graphicalindicatorcriteria/rowtype/) { get; } | Obtiene el valor del enum [`GraphicalIndicatorCriteriaType`](../graphicalindicatorcriteriatype/) que indica a qué filas se aplica el indicador. |
| [Test](../../aspose.tasks/graphicalindicatorcriteria/test/) { get; } | Obtiene el tipo de comparación realizado entre el valor del atributo extendido y los valores que actúan como criterio para la aplicación del indicador gráfico. [`FilterComparisonType`](../filtercomparisontype/) |
| [Value1](../../aspose.tasks/graphicalindicatorcriteria/value1/) { get; } | Obtiene el valor utilizado para probar el valor del atributo extendido. |
| [Value2](../../aspose.tasks/graphicalindicatorcriteria/value2/) { get; } | Obtiene el segundo valor utilizado para probar el valor del atributo extendido en caso de los tipos de comparación 'IsWithin' y 'IsNotWithin'. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [ToString](../../aspose.tasks/graphicalindicatorcriteria/tostring/)() | Devuelve la representación en cadena de la instancia de la clase `GraphicalIndicatorCriteria`. |

## Ejemplos

Muestra cómo recuperar la información de indicadores gráficos.

```csharp
Project project = new Project(DataDir + "graphical_indicators.mpp");

foreach (var ea in project.ExtendedAttributes)
{
    if (ea.GraphicalIndicator == null)
    {
        continue;
    }

    Console.WriteLine("GI for field '{0}':", ea.FieldName);

    foreach (var criterion in ea.GraphicalIndicator.Criteria)
    {
        Console.WriteLine("Row type: {0}", criterion.RowType);
        Console.WriteLine("Image index: {0}", criterion.ImageIndex);
        Console.Write(criterion.Test);
        if (criterion.Value1 != null)
        {
            Console.Write(" ");
            Console.Write(criterion.Value1.RawValue);
        }

        if (criterion.Value2 != null)
        {
            Console.Write(" ");
            Console.WriteLine(criterion.Value2.RawValue);
        }

        Console.WriteLine();
    }
}
```

Muestra cómo configurar un indicador gráfico para un atributo extendido.

```csharp
Project project = new Project();

var def = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, "Number field");
project.ExtendedAttributes.Add(def);
def.GraphicalIndicator = new GraphicalIndicatorsInfo();

GraphicalIndicatorCriteria criteria1 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsLessThan,
    2,
    new GraphicalIndicatorCriteriaValue(100m));

// El criterio 'IsWithin' requiere 2 valores.
GraphicalIndicatorCriteria criteria2 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsWithin,
    4,
    new GraphicalIndicatorCriteriaValue(101),
    new GraphicalIndicatorCriteriaValue(1000m));

// El criterio 'IsAnyValue' no requiere valores.
GraphicalIndicatorCriteria criteria3 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsAnyValue,
    4,
    null);

def.GraphicalIndicator.Criteria.Add(criteria1);
def.GraphicalIndicator.Criteria.Add(criteria2);
def.GraphicalIndicator.Criteria.Add(criteria3);

def.GraphicalIndicator.ProjectSummaryInheritFromNonSummaryRows = true;
def.GraphicalIndicator.SummaryRowsInheritFromNonSummaryRows = true;
def.GraphicalIndicator.ShowDataValuesInTooltip = false;

project.Save(OutDir + "CreateGraphicalIndicators_out.mpp", SaveFileFormat.Mpp);
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


