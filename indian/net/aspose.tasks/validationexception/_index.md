---
title: "क्लास ValidationException"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.ValidationException वर्ग। यह एक अपवाद का प्रतिनिधित्व करता है जो तब फेंका जाता है जब इकाई के वैधता परीक्षण के दौरान त्रुटियाँ पाई जाती हैं।"
type: docs
weight: 2790
url: /hi/net/aspose.tasks/validationexception/
---
## ValidationException class

इकाई के सत्यापन के दौरान त्रुटियों मिलने पर फेंके जाने वाले अपवाद का प्रतिनिधित्व करता है।

```csharp
public class ValidationException : ApplicationException
```

## उदाहरण

रिकरेंस टास्क के साथ काम करते समय &lt;see cref=\"ValidationException\"/&gt; को कैसे संभालें, दिखाता है।

```csharp
try
{
    var project = new Project();
    var parameters = new RecurringTaskParameters { TaskName = "t1", Duration = project.GetDuration(1, TimeUnitType.Day), RecurrencePattern = null };
    project.RootTask.Children.Add(parameters);
}
catch (ValidationException ex)
{
    Console.WriteLine("Message: ");
    Console.WriteLine(ex.Message);
    if (ex.InnerException != null)
    {
        Console.WriteLine("Inner exception message: ");
        Console.WriteLine(ex.InnerException.Message);
    }
}
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


