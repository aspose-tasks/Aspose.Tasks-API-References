---
title: "GroupCriterionCollection.CopyTo"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método GroupCriterionCollection. Copia los elementos de esta colección al array especificado comenzando en el índice de array especificado"
type: docs
weight: 60
url: /es/net/aspose.tasks/groupcriterioncollection/copyto/
---
## GroupCriterionCollection.CopyTo method

Copia los elementos de esta colección al array especificado, comenzando en el índice de array especificado.

```csharp
public void CopyTo(GroupCriterion[] array, int arrayIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arreglo | GroupCriterion[] | el arreglo unidimensional especificado al que copiar los elementos |
| arrayIndex | Int32 | el índice basado en cero del arreglo especificado en el que comienza la copia. |

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

* class [GroupCriterion](../../groupcriterion/)
* class [GroupCriterionCollection](../)
* namespace [Aspose.Tasks](../../groupcriterioncollection/)
* assembly [Aspose.Tasks](../../../)


