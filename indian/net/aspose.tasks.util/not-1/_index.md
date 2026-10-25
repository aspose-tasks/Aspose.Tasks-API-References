---
title: "क्लास NotT"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Util.Not1T क्लास। निर्दिष्ट शर्त पर लॉजिकल NOT लागू करता है"
type: docs
weight: 2750
url: /hi/net/aspose.tasks.util/not-1/
---
## Not&lt;T&gt; class

निर्दिष्ट शर्त पर लॉजिकल NOT लागू करता है।

```csharp
public class Not<T> : ICondition<T>
```

| पैरामीटर | विवरण |
| --- | --- |
| T | विधि इंटरफ़ेस लागू करने के लिए वस्तु का प्रकार। |

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [Not](not/)(ICondition&lt;T&gt;) | `Not` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Check](../../aspose.tasks.util/not-1/check/)(T) | यदि निर्दिष्ट ऑब्जेक्ट शर्त को पूरा करता है तो true लौटाता है। |

## उदाहरण

दिखाता है कि &lt;see cref="Aspose.Tasks.Util.Not`1" /&gt; शर्त का उपयोग कैसे करें।

```csharp
public void WorkWithNot()
{
    var project = new Project(DataDir + "Project2.mpp");

    // सभी प्रोजेक्ट टास्क इकट्ठा करें
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    // एक फ़िल्टर शर्त बनाएं
    var filter = new NullCondition();

    // और इसे <see cref="Aspose.Tasks.Util.Not`1" /> शर्त लागू करके उलटें
    var condition = new Not<Task>(filter);

    // एकत्रित कार्यों पर शर्त लागू करें
    List<Task> collection = Filter(coll.Tasks, condition);
    foreach (var task in collection)
    {
        Console.WriteLine("Name: " + task.Get(Tsk.Name));

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

private class NullCondition : ICondition<Task>
{
    public bool Check(Task el)
    {
        return el.Get(Tsk.IsNull).Value;
    }
}
```

### संबंधित देखें

* interface [ICondition&lt;T&gt;](../icondition-1/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


