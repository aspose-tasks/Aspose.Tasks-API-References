---
title: "Class RecalculationValidationException"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.RecalculationValidationException class. पुनर्गणना के बाद प्रोजेक्ट में त्रुटियों के मिलने पर फेंकी जाने वाली अपवाद को दर्शाता है"
type: docs
weight: 1680
url: /hi/net/aspose.tasks/recalculationvalidationexception/
---
## RecalculationValidationException class

पुनर्गणना के बाद प्रोजेक्ट में त्रुटियों मिलने पर फेंकी जाने वाली अपवाद को दर्शाता है।

```csharp
public abstract class RecalculationValidationException : ValidationException
```

## उदाहरण

दिखाता है कि किन स्थितियों में &lt;see cref=\"TaskValidationException\" /&gt; अपवाद फेंका जा सकता है।

```csharp
try
{
    var project = new Project { CalculationMode = CalculationMode.None };
    var task = project.RootTask.Children.Add("Task");

    // गलती से गलत तिथियां सेट कीं
    task.Set(Tsk.Start, new DateTime(2017, 6, 19, 8, 0, 0));
    task.Set(Tsk.Duration, project.GetDuration(1));
    task.Set(Tsk.Finish, new DateTime(2017, 6, 18, 17, 0, 0));

    // सत्यापन चलाने के लिए एक फ़्लैग के साथ प्रोजेक्ट पुनर्गणना चलाएँ   
    project.Recalculate(true);
}
catch (TaskValidationException ex)
{
    Console.WriteLine(ex.Message);
}
```

### संबंधित देखें

* class [ValidationException](../validationexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


