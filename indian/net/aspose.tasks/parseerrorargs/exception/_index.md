---
title: "ParseErrorArgs.Exception"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ParseErrorArgs प्रॉपर्टी। स्ट्रिंग मान को पार्स करते समय उत्पन्न अपवाद प्राप्त करता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks/parseerrorargs/exception/
---
## ParseErrorArgs.Exception property

स्ट्रिंग मान को पार्स करते समय उत्पन्न हुई अपवाद को प्राप्त करता है।

```csharp
public Exception Exception { get; }
```

## उदाहरण

अमान्य अक्षरों वाले XML फ़ाइल के साथ स्ट्रीम से प्रोजेक्ट पढ़ने का तरीका दिखाता है।

```csharp
public static void LoadProjectFromFile(string pathToModifiedXml)
{
    // टूटा हुआ टाइमस्पैन वाला XML शामिल करने वाली फ़ाइल खोलें
    var project = new Project(pathToModifiedXml, CustomDurationHandlerForFile2);
    Console.WriteLine(project.Get(Prj.Name));
}

public static object CustomDurationHandlerForFile2(object sender, ParseErrorArgs args)
{
    var regex = new Regex("[*]{2}(\\d+)Hrs(\\d+)Mins(\\d+)Secs[*]{2}");
    if (args.FieldType != typeof(TimeSpan))
    {
        throw args.Exception;
    }

    Console.WriteLine("Object field: {0}, Object field type: {1}, Invalid value: {2}", args.FieldName, args.FieldType, args.InvalidValue);
    var duration = regex.Replace(args.InvalidValue, "PT$1H$2M$3S");
    var newValue = Duration.ParseTimeSpan(duration);
    Console.WriteLine("New value : {0}", newValue);
    return newValue;
}
```

### संबंधित देखें

* class [ParseErrorArgs](../)
* namespace [Aspose.Tasks](../../parseerrorargs/)
* assembly [Aspose.Tasks](../../../)


