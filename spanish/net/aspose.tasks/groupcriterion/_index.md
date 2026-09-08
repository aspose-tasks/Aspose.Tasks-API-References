---
title: "Clase GroupCriterion"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.GroupCriterion class. Representa un criterio en una definición de grupo. El objeto GroupCriterion es un miembro de la colección GroupCriterionCollection."
type: docs
weight: 790
url: /es/net/aspose.tasks/groupcriterion/
---
## GroupCriterion class

Representa un criterio en una definición de grupo. El objeto GroupCriterion es un miembro de la colección [`GroupCriterionCollection`](../groupcriterioncollection/).

```csharp
public class GroupCriterion
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [GroupCriterion](groupcriterion/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Ascending](../../aspose.tasks/groupcriterion/ascending/) { get; set; } | Obtiene o establece un valor que indica si un campo usado como criterio en una definición de grupo está ordenado en orden ascendente. False si el campo está ordenado en orden descendente. |
| [CellColor](../../aspose.tasks/groupcriterion/cellcolor/) { get; set; } | Obtiene o establece el color del fondo de la celda para un campo usado como criterio en una definición de grupo. |
| [Field](../../aspose.tasks/groupcriterion/field/) { get; set; } | Obtiene o establece el campo por el cual se agrupa. |
| [Font](../../aspose.tasks/groupcriterion/font/) { get; set; } | Obtiene o establece la fuente para un criterio en una definición de grupo. |
| [FontColor](../../aspose.tasks/groupcriterion/fontcolor/) { get; set; } | Obtiene o establece el color de la fuente para un campo usado como criterio en una definición de grupo. |
| [GroupInterval](../../aspose.tasks/groupcriterion/groupinterval/) { get; set; } | Obtiene o establece el intervalo para un campo usado como criterio en una definición de grupo. |
| [GroupOn](../../aspose.tasks/groupcriterion/groupon/) { get; set; } | Obtiene o establece el tipo de agrupación para un campo usado como criterio en una definición de grupo. |
| [Pattern](../../aspose.tasks/groupcriterion/pattern/) { get; set; } | Obtiene o establece el patrón de la celda para un campo utilizado como criterio en una definición de grupo. |
| [StartAt](../../aspose.tasks/groupcriterion/startat/) { get; set; } | Obtiene o establece el inicio de los intervalos para un campo utilizado como criterio en una definición de grupo. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [Equals](../../aspose.tasks/groupcriterion/equals/)(object) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| override [GetHashCode](../../aspose.tasks/groupcriterion/gethashcode/)() | Funciona como una función hash para un tipo particular. |

## Ejemplos

Muestra cómo leer las propiedades de un criterio de grupo.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

Console.WriteLine("Task Groups Count: " + project.TaskGroups.Count);
var group = project.TaskGroups.ToList()[1];
Console.WriteLine("Task Group Name: " + group.Name);
Console.WriteLine("Task Group Criteria count: " + group.GroupCriteria.Count);

Console.WriteLine("\n************* Retrieving Task Group's Criterion information *************");
var criterion = group.GroupCriteria.ToList()[0];
Console.WriteLine("Task Criterion Field: " + criterion.Field);
Console.WriteLine("Task Criterion GroupOn: " + criterion.GroupOn);
Console.WriteLine("Task Criterion Cell Color: " + criterion.CellColor);
Console.WriteLine("Task Criterion Font Color: " + criterion.FontColor);
Console.WriteLine("Task Criterion Group Interval: " + criterion.GroupInterval);
Console.WriteLine("Task Criterion Start At: " + criterion.StartAt);

// Lee el patrón de fondo del criterio.
Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

Console.WriteLine("\n*********** Retrieving Criterion's Font Information ***********");
Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
Console.WriteLine("Font Size: " + criterion.Font.Size);
Console.WriteLine("Font Style: " + criterion.Font.Style);
Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
```

Muestra cómo agregar grupos a un proyecto.

```csharp
var p = new Project();

{
    var group = new Group();
    group.Name = "My new task group";
    group.MaintainHierarchy = true;
    group.ShowSummary = true;

    var criterion = new GroupCriterion();
    criterion.Field = Field.TaskDuration1;
    criterion.Font = new FontDescriptor("Comic Sans MS", 13F, FontStyles.Italic);
    criterion.GroupOn = GroupOn.DurationMinutes;
    criterion.StartAt = 5;
    criterion.GroupInterval = 3D;
    criterion.Pattern = BackgroundPattern.DarkDiagonalLeft;
    group.GroupCriteria.Add(criterion);

    var criterion2 = new GroupCriterion();
    criterion2.Field = Field.TaskPercentComplete;
    criterion2.Font = new FontDescriptor("Bodoni MT", 17, FontStyles.Italic | FontStyles.Bold);
    criterion2.GroupOn = GroupOn.Pct199;
    criterion2.Pattern = BackgroundPattern.LightDither;
    criterion2.CellColor = Color.Green;
    criterion2.FontColor = Color.Red;
    group.GroupCriteria.Add(criterion2);
    group.GroupAssignments = true;
    p.TaskGroups.Add(group);
}

{
    var group = new Group();
    group.Name = "My new resource group";
    group.MaintainHierarchy = true;
    group.ShowSummary = true;

    var criterion = new GroupCriterion();
    criterion.Field = Field.ResourceDuration1;
    criterion.Font = new FontDescriptor("Comic Sans MS", 11F, FontStyles.Bold);
    criterion.GroupOn = GroupOn.DurationHours;
    criterion.StartAt = 1;
    criterion.GroupInterval = 2D;
    criterion.Pattern = BackgroundPattern.DarkDiagonalLeft;
    group.GroupCriteria.Add(criterion);

    var criterion2 = new GroupCriterion();
    criterion2.Field = Field.ResourceCost;
    criterion2.Font = new FontDescriptor("Bodoni MT", 12, FontStyles.Italic | FontStyles.Bold);
    criterion2.GroupOn = GroupOn.Interval;
    criterion2.StartAt = 1D;
    criterion2.GroupInterval = 10D;
    criterion2.Pattern = BackgroundPattern.LightDither;
    criterion2.CellColor = Color.Magenta;
    criterion2.FontColor = Color.Red;
    group.GroupCriteria.Add(criterion2);
    group.GroupAssignments = true;
    p.ResourceGroups.Add(group);
}

p.Save(OutDir + "output_CreateGroup.mpp", new MPPSaveOptions() { WriteGroups = true });
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


