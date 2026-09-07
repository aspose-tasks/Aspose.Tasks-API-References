---
title: "क्लास GroupCriterionCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.GroupCriterionCollection क्लास। GroupCriterion ऑब्जेक्ट्स का संग्रह रखता है। ICollectionGroupCriterion इंटरफ़ेस को लागू करता है।"
type: docs
weight: 800
url: /hi/net/aspose.tasks/groupcriterioncollection/
---
## GroupCriterionCollection class

एक संग्रह जिसमें [`GroupCriterion`](../groupcriterion/) वस्तुएँ हैं। ICollection&lt;GroupCriterion&gt; इंटरफ़ेस को लागू करता है।

```csharp
public class GroupCriterionCollection : IList<GroupCriterion>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Count](../../aspose.tasks/groupcriterioncollection/count/) { get; } | इस संग्रह में मौजूद तत्वों की संख्या प्राप्त करता है। |
| [IsReadOnly](../../aspose.tasks/groupcriterioncollection/isreadonly/) { get; } | एक मान प्राप्त करता है जो दर्शाता है कि यह संग्रह केवल-रीड है या नहीं; अन्यथा, false। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Add](../../aspose.tasks/groupcriterioncollection/add/)(GroupCriterion) | निर्दिष्ट आइटम को इस संग्रह में जोड़ता है। |
| [Clear](../../aspose.tasks/groupcriterioncollection/clear/)() | इस संग्रह से सभी आइटम हटाता है। |
| [Contains](../../aspose.tasks/groupcriterioncollection/contains/)(GroupCriterion) | यदि निर्दिष्ट आइटम इस संग्रह में पाया जाता है तो true लौटाता है; अन्यथा false। |
| [CopyTo](../../aspose.tasks/groupcriterioncollection/copyto/)(GroupCriterion[], int) | निर्दिष्ट एरे सूचकांक से शुरू करके इस संग्रह के तत्वों को निर्दिष्ट एरे में कॉपी करता है। |
| [GetEnumerator](../../aspose.tasks/groupcriterioncollection/getenumerator/)() | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [Remove](../../aspose.tasks/groupcriterioncollection/remove/)(GroupCriterion) | इस संग्रह से विशिष्ट वस्तु की पहली घटना को हटाता है। |
| [ToList](../../aspose.tasks/groupcriterioncollection/tolist/)() | एक GroupCriterion संग्रह को [`GroupCriterion`](../groupcriterion/) वस्तुओं की सूची में परिवर्तित करता है। |

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

* class [GroupCriterion](../groupcriterion/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


