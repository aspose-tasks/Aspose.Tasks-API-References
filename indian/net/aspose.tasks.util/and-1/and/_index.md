---
title: "And1.And"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "And constructor. And वर्ग का नया उदाहरण आरंभ करता है।"
type: docs
weight: 10
url: /hi/net/aspose.tasks.util/and-1/and/
---
## And&lt;T&gt; constructor

[`And`](../) वर्ग का नया उदाहरण आरंभ करता है।

```csharp
public And(ICondition<T> cond1, ICondition<T> cond2)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| cond1 | ICondition`1 | पहली शर्त। |
| cond2 | ICondition`1 | दूसरी शर्त। |

## उदाहरण

दिखाता है कि &lt;see cref="Aspose.Tasks.Util.And`1" /&gt; शर्त का उपयोग कैसे करें।

```csharp
public void WorkWithAnd()
{
    var project = new Project(DataDir + "Project2.mpp");

    // सभी प्रोजेक्ट टास्क इकट्ठा करें
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    // एक फ़िल्टर शर्त बनाएं जो सारांश कार्यों को फ़िल्टर करती है
    var condition1 = new SummaryCondition();

    // एक फ़िल्टर शर्त बनाएं जो नॉन-नल कार्यों को फ़िल्टर करती है
    var condition2 = new NotNullCondition();

    // और उन्हें <see cref="Aspose.Tasks.Util.And`1" /> शर्त लागू करके जोड़ें
    var joinedCondition = new And<Task>(condition1, condition2);

    // एकत्रित कार्यों पर शर्त लागू करें
    List<Task> collection = Filter(coll.Tasks, joinedCondition);
    Console.WriteLine("Filtered tasks: ");
    foreach (var task in collection)
    {
        Console.WriteLine(" Name: " + task.Get(Tsk.Name));

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
* class [And&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../and-1/)
* assembly [Aspose.Tasks](../../../)


