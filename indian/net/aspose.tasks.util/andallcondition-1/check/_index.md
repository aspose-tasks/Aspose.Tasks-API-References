---
title: "AndAllCondition1.Check"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "AndAllCondition मेथड। यदि निर्दिष्ट ऑब्जेक्ट शर्तों को पूरा करता है तो true लौटाता है।"
type: docs
weight: 20
url: /hi/net/aspose.tasks.util/andallcondition-1/check/
---
## AndAllCondition&lt;T&gt;.Check method

यदि निर्दिष्ट ऑब्जेक्ट शर्तों को पूरा करता है तो true लौटाता है।

```csharp
public bool Check(T el)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| el | T | जाँचने के लिए वस्तु। |

### रिटर्न वैल्यू

यदि वस्तु शर्तों को पूरा करती है तो सत्य।

## उदाहरण

दिखाता है कि कैसे &lt;see cref=\"Aspose.Tasks.Util.AndAllCondition`1\" /&gt; शर्त का उपयोग किया जाए।

```csharp
public void WorkWithAndAllCondition()
{
    var project = new Project(DataDir + "Project2.mpp");

    // सभी प्रोजेक्ट टास्क इकट्ठा करें
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    var conditions = new List<ICondition<Task>>
                         {
                             // एक फ़िल्टर शर्त बनाएं जो नॉन-नल कार्यों को फ़िल्टर करती है
                             new NotNullCondition(),

                             // एक फ़िल्टर शर्त बनाएं जो सारांश कार्यों को फ़िल्टर करती है
                             new SummaryCondition()
                         };

    // और उन्हें <see cref=\"Aspose.Tasks.Util.AndAllCondition`1\" /> शर्त लागू करके जोड़ें
    var joinedCondition = new AndAllCondition<Task>(conditions);

    // एकत्रित कार्यों पर शर्त लागू करें
    List<Task> collection = Filter(coll.Tasks, joinedCondition);
    Console.WriteLine("Filtered tasks: ");
    foreach (var task in collection)
    {
        Console.WriteLine("  Name: " + task.Get(Tsk.Name));

        // अन्य गुणों के साथ काम करें...
    }

    // ...
}

private static List<T> Filter<T>(IEnumerable<T> array, ICondition<T> cond)
{
    var result = new List<T>();

    foreach (var item in array)
    {
        if (cond.Check(item))
        {
            result.Add(item);
        }
    }

    return result;
}

private class NotNullCondition : ICondition<Task>
{
    public bool Check(Task el)
    {
        return !el.Get(Tsk.IsNull).Value;
    }
}

private class SummaryCondition : ICondition<Task>
{
    public bool Check(Task el)
    {
        return el.Get(Tsk.IsSummary);
    }
}
```

### संबंधित देखें

* class [AndAllCondition&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../andallcondition-1/)
* assembly [Aspose.Tasks](../../../)


