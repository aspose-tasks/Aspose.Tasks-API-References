---
title: "डेलीगेट ParseErrorCallback"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "एक मेथड कॉलबैक को दर्शाता है जो XML डेटा पढ़ते समय हो सकने वाली पार्स त्रुटियों को संभालता है"
type: docs
weight: 1250
url: /hi/net/aspose.tasks/parseerrorcallback/
---
## ParseErrorCallback delegate

XML डेटा पढ़ते समय हो सकने वाली पार्स त्रुटियों को संभालने के लिए एक मेथड कॉलबैक का प्रतिनिधित्व करता है।

```csharp
public delegate object ParseErrorCallback(object sender, ParseErrorArgs args);
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रेषक | ऑब्जेक्ट | पार्स त्रुटि का स्रोत ऑब्जेक्ट। |
| args | ParseErrorArgs | इवेंट डेटा शामिल करने वाले [`ParseErrorArgs`](../parseerrorargs/) क्लास का इंस्टेंस। |

### रिटर्न वैल्यू

निर्दिष्ट प्रेषक ऑब्जेक्ट पर सेट करने के लिए परिवर्तित मान।

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

* class [ParseErrorArgs](../parseerrorargs/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


