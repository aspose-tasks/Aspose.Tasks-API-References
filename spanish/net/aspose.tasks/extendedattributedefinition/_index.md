---
title: "Clase ExtendedAttributeDefinition"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.ExtendedAttributeDefinition. Representa una definición de atributo extendido asociado a un proyecto"
type: docs
weight: 540
url: /es/net/aspose.tasks/extendedattributedefinition/
---
## ExtendedAttributeDefinition class

Representa una definición de atributo extendido asociada a un proyecto.

```csharp
public class ExtendedAttributeDefinition
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Alias](../../aspose.tasks/extendedattributedefinition/alias/) { get; set; } | Obtiene o establece el alias de un campo personalizado. |
| [AppendNewValues](../../aspose.tasks/extendedattributedefinition/appendnewvalues/) { get; set; } | Obtiene o establece un valor que indica si los nuevos valores agregados a un proyecto se añaden automáticamente a la lista. |
| [AutoRollDown](../../aspose.tasks/extendedattributedefinition/autorolldown/) { get; set; } | Obtiene o establece un valor que indica si se habilita una propagación automática a asignaciones. |
| [CalculationType](../../aspose.tasks/extendedattributedefinition/calculationtype/) { get; set; } | Obtiene o establece el tipo de cálculo del valor del atributo personalizado. |
| [CfType](../../aspose.tasks/extendedattributedefinition/cftype/) { get; } | Obtiene el tipo de un campo personalizado. |
| [Default](../../aspose.tasks/extendedattributedefinition/default/) { get; set; } | Obtiene o establece el valor predeterminado en la lista. |
| [DefaultGuid](../../aspose.tasks/extendedattributedefinition/defaultguid/) { get; set; } | Obtiene o establece el GUID de la entrada predeterminada de la tabla de búsqueda. |
| [ElementType](../../aspose.tasks/extendedattributedefinition/elementtype/) { get; set; } | Obtiene o establece si el atributo extendido está asociado a una tarea, un recurso o una asignación. |
| [FieldId](../../aspose.tasks/extendedattributedefinition/fieldid/) { get; set; } | Obtiene o establece la correspondencia al id del proyecto de un campo personalizado. Use la representación en cadena de una constante de la clase [`ExtendedAttributeTask`](../extendedattributetask/) para especificar la propiedad [`FieldId`](./fieldid/). |
| [FieldName](../../aspose.tasks/extendedattributedefinition/fieldname/) { get; } | Obtiene el nombre de un campo personalizado. |
| [Formula](../../aspose.tasks/extendedattributedefinition/formula/) { get; set; } | Obtiene o establece la fórmula que Microsoft Project usa para rellenar un campo de tarea personalizado. |
| [GraphicalIndicator](../../aspose.tasks/extendedattributedefinition/graphicalindicator/) { get; set; } | Obtiene o establece la información de indicadores gráficos asociada al atributo extendido. Aplicable al formato MPP. |
| [Guid](../../aspose.tasks/extendedattributedefinition/guid/) { get; set; } | Obtiene o establece el GUID de un campo personalizado. |
| [LookupUid](../../aspose.tasks/extendedattributedefinition/lookupuid/) { get; } | Obtiene un GUID de la tabla de búsqueda asociada a un campo personalizado. |
| [MaxMultiValues](../../aspose.tasks/extendedattributedefinition/maxmultivalues/) { get; set; } | Obtiene o establece el número máximo de valores que puede establecer en una lista de selección. |
| [ParentProject](../../aspose.tasks/extendedattributedefinition/parentproject/) { get; } | Obtiene el proyecto principal para la instancia `ExtendedAttributeDefinition`. |
| [PhoneticsAlias](../../aspose.tasks/extendedattributedefinition/phoneticsalias/) { get; set; } | Obtiene o establece la pronunciación fonética del alias de un campo personalizado. |
| [RestrictValues](../../aspose.tasks/extendedattributedefinition/restrictvalues/) { get; set; } | Obtiene o establece un valor que indica si los valores del campo personalizado están restringidos a los valores de la [`ValueList`](./valuelist/). |
| [RollupType](../../aspose.tasks/extendedattributedefinition/rolluptype/) { get; set; } | Obtiene o establece la forma en que se calculan los acumulados. |
| [SecondaryGuid](../../aspose.tasks/extendedattributedefinition/secondaryguid/) { get; set; } | Obtiene o establece el GUID secundario del atributo extendido. |
| [SecondaryPid](../../aspose.tasks/extendedattributedefinition/secondarypid/) { get; set; } | Obtiene o establece el PID secundario de un campo personalizado. |
| [SummaryRowsCalculationType](../../aspose.tasks/extendedattributedefinition/summaryrowscalculationtype/) { get; set; } | Obtiene o establece el tipo de cálculo del valor del atributo personalizado para filas de resumen. |
| [UserDef](../../aspose.tasks/extendedattributedefinition/userdef/) { get; set; } | Obtiene o establece un valor que indica si un campo personalizado es definido por el usuario. |
| [ValueList](../../aspose.tasks/extendedattributedefinition/valuelist/) { get; } | Obtiene la lista List&lt;Value&gt; ValueList. |
| [ValuelistSortOrder](../../aspose.tasks/extendedattributedefinition/valuelistsortorder/) { get; set; } | Obtiene o establece la forma en que se ordenan las listas de valores. Los valores son: 0=Descendente, 1=Ascendente. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/#createlookupresourcedefinition_1)(ExtendedAttributeResource, string) | Método de fábrica que crea una definición de atributo extendido con búsqueda. Tiene [`CalculationType`](./calculationtype/) igual a Lookup y solo se puede usar en Recursos. Se requiere especificar *fieldId* y *alias* al llamar a este método. El tipo de campo se infiere del id del campo. |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/#createlookupresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Método de fábrica que crea una definición de atributo extendido con búsqueda. Tiene [`CalculationType`](./calculationtype/) igual a Lookup y solo se puede usar en Recursos. Se requiere especificar *customFieldType*, *fieldId* y *alias* al llamar a este método. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/#createlookuptaskdefinition_1)(ExtendedAttributeTask, string) | Método de fábrica que crea una definición de atributo extendido con búsqueda. Tiene [`CalculationType`](./calculationtype/) igual a Lookup y solo se puede usar en Tareas. Se requiere especificar *fieldId* y *alias* al llamar a este método. El tipo de campo se infiere del id del campo. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/#createlookuptaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Método de fábrica que crea una definición de atributo extendido con búsqueda. Tiene [`CalculationType`](./calculationtype/) igual a Lookup y solo se puede usar en Tareas. Se requiere especificar *customFieldType*, *fieldId* y *alias* al llamar a este método. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition/#createresourcedefinition_1)(ExtendedAttributeResource, string) | Método de fábrica que crea una definición de atributo extendido simple, que Microsoft Project muestra como \"None\". Tiene [`CalculationType`](./calculationtype/) igual a None y solo se puede usar en Recursos. Se requiere especificar *fieldId* y *alias* al llamar a este método. El tipo de campo se infiere del id del campo. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition/#createresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Método de fábrica que crea una definición de atributo extendido simple, que Microsoft Project muestra como \"None\". Tiene [`CalculationType`](./calculationtype/) igual a None y solo se puede usar en Recursos. Se requiere especificar *customFieldType*, *fieldId* y *alias* al llamar a este método. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition/#createtaskdefinition_1)(ExtendedAttributeTask, string) | Método de fábrica que crea una definición de atributo extendido simple, que Microsoft Project muestra como \"None\". Tiene [`CalculationType`](./calculationtype/) igual a None y solo se puede usar en Tareas. Se requiere especificar *fieldId* y *alias* al llamar a este método. El tipo de campo se infiere del id del campo. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition/#createtaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Método de fábrica que crea una definición de atributo extendido simple, que Microsoft Project muestra como \"None\". Tiene [`CalculationType`](./calculationtype/) igual a None y solo se puede usar en Tareas. Se requiere especificar *customFieldType*, *fieldId* y *alias* al llamar a este método. |
| [AddLookupValue](../../aspose.tasks/extendedattributedefinition/addlookupvalue/)(Value) | Añade un valor a la lista de búsqueda interna. Esta es la forma preferida para manipular la [`ValueList`](./valuelist/). |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute)() | Crea un nuevo atributo extendido con el ID de campo que es igual al valor del ID de campo de este objeto. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_3)(bool) | Crea un nuevo atributo extendido con el ID de campo que es igual al valor del ID de campo de este objeto y el valor de bandera especificado. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_4)(DateTime) | Crea un nuevo atributo extendido con el ID de campo que es igual al valor del ID de campo de este objeto y el valor de fecha especificado. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_5)(decimal) | Crea un nuevo atributo extendido con el ID de campo que es igual al valor del ID de campo de este objeto y el valor numérico especificado. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_1)(Duration) | Crea un nuevo atributo extendido con el ID de campo que es igual al valor del ID de campo de este objeto y el valor de duración especificado. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_6)(string) | Crea un nuevo atributo extendido con el ID de campo que es igual al valor del ID de campo de este objeto y el valor de texto especificado. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_2)(Value) | Crea un nuevo atributo extendido vinculado al elemento [`Value`](../value/) especificado. |
| override [Equals](../../aspose.tasks/extendedattributedefinition/equals/)(object) | Devuelve una bandera que indica si esta instancia es igual al objeto especificado. |
| override [GetHashCode](../../aspose.tasks/extendedattributedefinition/gethashcode/)() | Devuelve un código hash para la instancia de la clase `ExtendedAttributeDefinition`. |
| [RemoveLookupValue](../../aspose.tasks/extendedattributedefinition/removelookupvalue/)(Value) | Elimina un valor de la lista interna de búsqueda. Esta es una forma preferible de manipular la [`ValueList`](./valuelist/). |

## Ejemplos

Muestra cómo usar funciones matemáticas comunes con atributos extendidos.

```csharp
public static void EvaluateChoose()
{
    var project = CreateTestProjectWithCustomField();

    // Establecer fórmula
    project.ExtendedAttributes[0].Formula = "Choose(3, \"This is a\", \"right\", \"choice\")";

    // Imprimir valor del atributo extendido
    var task = project.RootTask.Children.GetById(1);
    Console.WriteLine(task.ExtendedAttributes[0].TextValue);
}

public static void EvaluateIsNumeric()
{
    string[] numericFormulas =
        {
            "IsNumeric('AAA')", @"IsNUmeric(1)", "IsNumeric(1<0)", "IsNumeric(\"1.1\")", "IsNumeric(Choose((2 + Sgn(2^-3)), 123, \"one two three\"))"
        };

    var project = CreateTestProjectWithCustomField();

    foreach (var numericFormula in numericFormulas)
    {
        // Establecer fórmula
        project.ExtendedAttributes[0].Formula = numericFormula;

        // Imprimir valor del atributo extendido
        var task = project.RootTask.Children.GetById(1);
        Console.WriteLine(task.ExtendedAttributes[0].TextValue);
    }
}

public static void EvaluateSwitch()
{
    var project = CreateTestProjectWithCustomField();

    // Establecer fórmula
    project.ExtendedAttributes[0].Formula = "Switch( 0 < 1, \"0 is lesser than 1\", 0 > 1, \"0 is greater than 1\")";

    // Imprimir valor del atributo extendido
    var task = project.RootTask.Children.GetById(1);
    Console.WriteLine(task.ExtendedAttributes[0].TextValue);
}

public static Project CreateTestProjectWithCustomField()
{
    var project = new Project();
    var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Custom Field");
    project.ExtendedAttributes.Add(definition);

    var task = project.RootTask.Children.Add("Task");

    var attribute = definition.CreateExtendedAttribute();
    task.ExtendedAttributes.Add(attribute);
    return project;
}
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


