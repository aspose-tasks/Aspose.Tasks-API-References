---
title: "क्लास InvalidPasswordException"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.InvalidPasswordException क्लास। वह अपवाद प्रकार दर्शाता है जो गलत पासवर्ड के साथ पासवर्ड-संरक्षित फ़ाइल खोलने पर फेंका जाता है।"
type: docs
weight: 910
url: /hi/net/aspose.tasks/invalidpasswordexception/
---
## InvalidPasswordException class

गलत पासवर्ड के साथ पासवर्ड-संरक्षित फ़ाइल खोलने पर फेंकी जाने वाली अपवाद प्रकार का प्रतिनिधित्व करता है।

```csharp
public class InvalidPasswordException : TasksException
```

## उदाहरण

पासवर्ड-संरक्षित प्रोजेक्ट फ़ाइलें पढ़ते समय &lt;see cref=\"InvalidPasswordException\"/&gt; को संभालने का तरीका दर्शाता है।

```csharp
try
{
    var project = new Project(DataDir + "PasswordProtected.mpp");

    // प्रोजेक्ट के साथ काम करना ...
    Console.WriteLine("Project Name: " + project.Get(Prj.Name));
}
catch (TasksReadingException e)
{
    // संदेश है \"प्रोजेक्ट पासवर्ड-संरक्षित है। पासवर्ड प्रदान नहीं किया गया है या गलत है।\"
    Console.WriteLine(e.Message);
}
```

### संबंधित देखें

* class [TasksException](../tasksexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


