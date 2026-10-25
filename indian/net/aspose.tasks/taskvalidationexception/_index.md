---
title: "क्लास TaskValidationException"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.TaskValidationException क्लास। यह एक अपवाद का प्रतिनिधित्व करता है जो पुनर्गणना के बाद प्रोजेक्ट कार्यों में त्रुटियों के मिलने पर फेंका जाता है"
type: docs
weight: 2510
url: /hi/net/aspose.tasks/taskvalidationexception/
---
## TaskValidationException class

पुनर्गणना के बाद प्रोजेक्ट के कार्यों में त्रुटियाँ मिलने पर फेंके जाने वाले अपवाद का प्रतिनिधित्व करता है।

```csharp
public class TaskValidationException : RecalculationValidationException
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Task](../../aspose.tasks/taskvalidationexception/task/) { get; } | उस कार्य को प्राप्त करता है जिसने अपवाद उत्पन्न किया। |

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

* class [RecalculationValidationException](../recalculationvalidationexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


