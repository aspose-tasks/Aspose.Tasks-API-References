---
title: "Asn.BudgetWork"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Asn फ़ील्ड। असाइनमेंट पर कार्य या सामग्री संसाधनों के लिए बजटेड कार्य मात्रा"
type: docs
weight: 160
url: /hi/net/aspose.tasks/asn/budgetwork/
---
## Asn.BudgetWork field

असाइनमेंट पर कार्य या सामग्री संसाधनों के लिए बजटेड कार्य मात्रा।

```csharp
public static readonly Key<Duration, AsnKey> BudgetWork;
```

## उदाहरण

दिखाता है कि संसाधन असाइनमेंट के बजट कार्य/लागत मान कैसे पढ़ें।

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
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


