---
title: "GroupCriterionCollection.CopyTo"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "GroupCriterionCollection मेथड। इस संग्रह के तत्वों को निर्दिष्ट एरे में निर्दिष्ट एरे इंडेक्स से शुरू करके कॉपी करता है"
type: docs
weight: 60
url: /hi/net/aspose.tasks/groupcriterioncollection/copyto/
---
## GroupCriterionCollection.CopyTo method

निर्दिष्ट एरे सूचकांक से शुरू करके इस संग्रह के तत्वों को निर्दिष्ट एरे में कॉपी करता है।

```csharp
public void CopyTo(GroupCriterion[] array, int arrayIndex)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| एरे | GroupCriterion[] | तत्वों को कॉपी करने के लिए निर्दिष्ट एक-आयामी एरे |
| arrayIndex | Int32 | निर्दिष्ट एरे का शून्य-आधारित इंडेक्स जहाँ से कॉपी शुरू होती है। |

## उदाहरण

समूह मानदंड के संग्रह के साथ काम करने का तरीका दर्शाता है।

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

var group = project.TaskGroups.ToList()[0];

// समूह मानदंड पर पुनरावृति करें
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

// मानदंड को अन्य समूह में कॉपी करें
var otherGroup = project.TaskGroups.ToList()[0];

var criteria = new GroupCriterion[group.GroupCriteria.Count];
group.GroupCriteria.CopyTo(criteria, 0);
foreach (var criterion in criteria)
{
    otherGroup.GroupCriteria.Add(criterion);
}
```

### संबंधित देखें

* class [GroupCriterion](../../groupcriterion/)
* class [GroupCriterionCollection](../)
* namespace [Aspose.Tasks](../../groupcriterioncollection/)
* assembly [Aspose.Tasks](../../../)


