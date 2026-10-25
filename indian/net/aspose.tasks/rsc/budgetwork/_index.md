---
title: "Rsc.BudgetWork"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। बजट कार्य बजट कार्य और सामग्री संसाधनों के लिए। बजट संसाधनों को केवल प्रोजेक्ट सारांश कार्य को सौंपा जाता है।"
type: docs
weight: 180
url: /hi/net/aspose.tasks/rsc/budgetwork/
---
## Rsc.BudgetWork field

बजट कार्य बजट कार्य और सामग्री संसाधनों के लिए। बजट संसाधनों को केवल परियोजना सारांश कार्य को सौंपा जाता है।

```csharp
public static readonly Key<Duration, RscKey> BudgetWork;
```

## उदाहरण

एक संसाधन के बजट कार्य/लागत मानों को पढ़ने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

// प्रोजेक्ट सारांश कार्य के लिए बजट कार्य और बजट लागत प्रदर्शित करें।
Console.WriteLine("projSummary.BudgetWork = " + project.RootTask.Get(Tsk.BudgetWork));
Console.WriteLine("projSummary.BudgetCost = " + project.RootTask.Get(Tsk.BudgetCost));

// संसाधन बजट कार्य प्रदर्शित करें।
var rsc = project.Resources.GetByUid(6);
Console.WriteLine("Resource BudgetWork = " + rsc.Get(Rsc.BudgetWork));

// संसाधन बजट लागत प्रदर्शित करें।
rsc = project.Resources.GetByUid(7);
Console.WriteLine("Resource BudgetCost = " + rsc.Get(Rsc.BudgetCost));

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // असाइनमेंट बजट कार्य और बजट लागत प्रदर्शित करें।
    foreach (var assignment in task.Assignments)
    {
        var resource = assignment.Get(Asn.Resource);
        if (resource == null)
        {
            continue;
        }

        if (resource.Get(Rsc.Type) == ResourceType.Work)
        {
            Console.WriteLine("Assignment BudgetWork = " + assignment.Get(Asn.BudgetWork));
        }
        else
        {
            Console.WriteLine("Assignment BudgetCost = " + assignment.Get(Asn.BudgetCost));
        }
    }
}
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


