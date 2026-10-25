---
title: "Clase GraphicalIndicatorCriteriaValue"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.GraphicalIndicatorCriteriaValue. Representa un valor usado en la verificación de condiciones de los criterios de indicadores gráficos"
type: docs
weight: 750
url: /es/net/aspose.tasks/graphicalindicatorcriteriavalue/
---
## GraphicalIndicatorCriteriaValue class

Representa un valor utilizado en la verificación de condición de los criterios de indicadores gráficos.

```csharp
public sealed class GraphicalIndicatorCriteriaValue
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_1)(bool) | Crea una instancia de la clase GraphicalIndicatorCriteriaValue con un valor constante de bandera (bool). |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_2)(DateTime) | Crea una instancia de la clase GraphicalIndicatorCriteriaValue con un valor constante de DateTime. |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_3)(decimal) | Crea una instancia de la clase GraphicalIndicatorCriteriaValue con un valor constante decimal. |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor)(Duration) | Crea una instancia de la clase GraphicalIndicatorCriteriaValue con un valor constante de Duration. |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_4)(string) | Crea una instancia de la clase GraphicalIndicatorCriteriaValue con un valor constante de cadena. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [IsFieldLink](../../aspose.tasks/graphicalindicatorcriteriavalue/isfieldlink/) { get; } | Obtiene si la instancia actual es un enlace de campo (representa un valor de un campo). |
| [RawValue](../../aspose.tasks/graphicalindicatorcriteriavalue/rawvalue/) { get; } | Obtiene la constante subyacente del valor Field. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [CreateFieldLink](../../aspose.tasks/graphicalindicatorcriteriavalue/createfieldlink/)(Field) | Crea una instancia de la clase GraphicalIndicatorCriteriaValue que representa el valor del campo especificado de MS Project. |
| override [ToString](../../aspose.tasks/graphicalindicatorcriteriavalue/tostring/)() | Devuelve una cadena que representa el objeto actual. |

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


