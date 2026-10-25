---
title: "Tsk.BudgetWork"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। बजट कार्य और सामग्री संसाधनों के लिए बजट कार्य। बजट संसाधन केवल प्रोजेक्ट सारांश कार्य को सौंपे जाते हैं।"
type: docs
weight: 150
url: /hi/net/aspose.tasks/tsk/budgetwork/
---
## Tsk.BudgetWork field

बजट कार्य बजट कार्य और सामग्री संसाधनों के लिए। बजट संसाधन केवल प्रोजेक्ट सारांश टास्क को सौंपे जाते हैं।

```csharp
public static readonly Key<Duration, TaskKey> BudgetWork;
```

## उदाहरण

दिखाता है कि कार्य/संसाधन/असाइनमेंट के बजट कार्य/लागत मानों को कैसे पढ़ें।

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
foreach (var tsk in collector.Tasks)
{
    // असाइनमेंट बजट कार्य और बजट लागत प्रदर्शित करें।
    foreach (var assignment in tsk.Assignments)
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
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


