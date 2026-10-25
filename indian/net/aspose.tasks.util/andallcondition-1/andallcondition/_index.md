---
title: "AndAllCondition1.AndAllCondition"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "AndAllCondition कंस्ट्रक्टर। AndAllCondition क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।"
type: docs
weight: 10
url: /hi/net/aspose.tasks.util/andallcondition-1/andallcondition/
---
## AndAllCondition&lt;T&gt; constructor

[`AndAllCondition`](../) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

```csharp
public AndAllCondition(List<ICondition<T>> conditions)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| शर्तें | List`1 | शर्तों की सूची। |

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

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [AndAllCondition&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../andallcondition-1/)
* assembly [Aspose.Tasks](../../../)


