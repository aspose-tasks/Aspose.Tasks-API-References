---
title: "क्लास AndAllConditionT"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Util.AndAllCondition1T क्लास। सभी शर्तों पर लॉजिकल AND लागू करता है। उदाहरण के लिए cond1 AND cond2 AND cond3"
type: docs
weight: 2660
url: /hi/net/aspose.tasks.util/andallcondition-1/
---
## AndAllCondition&lt;T&gt; class

सभी शर्तों पर लॉजिकल AND लागू करता है। उदाहरण के लिए: cond1 AND cond2 AND cond3...

```csharp
public class AndAllCondition<T> : ICondition<T>
```

| पैरामीटर | विवरण |
| --- | --- |
| T | विधि इंटरफ़ेस लागू करने के लिए वस्तु का प्रकार। |

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [AndAllCondition](andallcondition/)(List&lt;ICondition&lt;T&gt;&gt;) | `AndAllCondition` क्लास का एक नया इंस्टेंस प्रारंभ करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Check](../../aspose.tasks.util/andallcondition-1/check/)(T) | यदि निर्दिष्ट ऑब्जेक्ट शर्तों को पूरा करता है तो true लौटाता है। |

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

* interface [ICondition&lt;T&gt;](../icondition-1/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


