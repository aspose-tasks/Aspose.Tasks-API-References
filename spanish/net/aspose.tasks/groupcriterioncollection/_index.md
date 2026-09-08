---
title: "Clase GroupCriterionCollection"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.GroupCriterionCollection. Contiene una colección de objetos GroupCriterion. Implementa la interfaz ICollectionGroupCriterion."
type: docs
weight: 800
url: /es/net/aspose.tasks/groupcriterioncollection/
---
## GroupCriterionCollection class

Contiene una colección de objetos [`GroupCriterion`](../groupcriterion/). Implementa la interfaz ICollection&lt;GroupCriterion&gt;.

```csharp
public class GroupCriterionCollection : IList<GroupCriterion>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.tasks/groupcriterioncollection/count/) { get; } | Obtiene el número de elementos contenidos en esta colección. |
| [IsReadOnly](../../aspose.tasks/groupcriterioncollection/isreadonly/) { get; } | Obtiene un valor que indica si esta colección es de solo lectura; de lo contrario, false. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.tasks/groupcriterioncollection/add/)(GroupCriterion) | Agrega el elemento especificado a esta colección. |
| [Clear](../../aspose.tasks/groupcriterioncollection/clear/)() | Elimina todos los elementos de esta colección. |
| [Contains](../../aspose.tasks/groupcriterioncollection/contains/)(GroupCriterion) | Devuelve true si el elemento especificado se encuentra en esta colección; de lo contrario, false. |
| [CopyTo](../../aspose.tasks/groupcriterioncollection/copyto/)(GroupCriterion[], int) | Copia los elementos de esta colección al array especificado, comenzando en el índice de array especificado. |
| [GetEnumerator](../../aspose.tasks/groupcriterioncollection/getenumerator/)() | Devuelve un enumerador para esta colección. |
| [Remove](../../aspose.tasks/groupcriterioncollection/remove/)(GroupCriterion) | Elimina la primera aparición de un objeto específico de esta colección. |
| [ToList](../../aspose.tasks/groupcriterioncollection/tolist/)() | Convierte una colección de GroupCriterion en una lista de objetos [`GroupCriterion`](../groupcriterion/). |

## Ejemplos

Muestra cómo trabajar con una colección de criterios de grupo.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

var group = project.TaskGroups.ToList()[0];

// iterar sobre criterios de grupo
Console.WriteLine("Print group criteria of the group '{0}': ", group.Name);
Console.WriteLine("Group criterion count: " + group.GroupCriteria.Count);
foreach (var criterion in group.GroupCriteria)
{
    Console.WriteLine("Field: " + criterion.Field);
    Console.WriteLine("Group On: " + criterion.GroupOn);
    Console.WriteLine();
}

group.GroupCriteria.Clear();

if (!group.GroupCriteria.IsReadOnly)
{
    List<GroupCriterion> groupCriteria = group.GroupCriteria.ToList();
    foreach (var criterion in groupCriteria)
    {
        group.GroupCriteria.Remove(criterion);
    }
}

var criterionToAdd = new GroupCriterion
{
    Ascending = true,
    Field = Field.TaskActive
};

if (!group.GroupCriteria.Contains(criterionToAdd))
{
    group.GroupCriteria.Add(criterionToAdd);
}

// copiar criterios a otro grupo
var otherGroup = project.TaskGroups.ToList()[0];

var criteria = new GroupCriterion[group.GroupCriteria.Count];
group.GroupCriteria.CopyTo(criteria, 0);
foreach (var criterion in criteria)
{
    otherGroup.GroupCriteria.Add(criterion);
}
```

### Ver también

* class [GroupCriterion](../groupcriterion/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


