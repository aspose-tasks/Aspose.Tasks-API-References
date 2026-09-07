---
title: "LoadOptions.ErrorHandler"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "LoadOptions प्रॉपर्टी। XML पार्स त्रुटियों को संभालने के लिए एक कॉलबैक मेथड प्राप्त करता या सेट करता है"
type: docs
weight: 40
url: /hi/net/aspose.tasks/loadoptions/errorhandler/
---
## LoadOptions.ErrorHandler property

XML पार्स त्रुटियों को संभालने के लिए कॉलबैक मेथड को प्राप्त करता है या सेट करता है।

```csharp
public ParseErrorCallback ErrorHandler { get; set; }
```

## उदाहरण

दिखाता है कि कैसे एक Primavera XML फ़ाइल से त्रुटि पार्सिंग के साथ प्रोजेक्ट पढ़ा जाए।

```csharp
var options = new PrimaveraReadOptions
{
    ProjectUid = 4557
};

var loadOptions = new LoadOptions()
{
    PrimaveraReadOptions = options,
    ErrorHandler = CustomDurationHandlerForFile
};

// विशेष UID वाला प्रोजेक्ट लौटाता है।
var project = new Project(OutDir + "IgnoreInvalidCharacters_out.xml", loadOptions);
Console.WriteLine(project.Get(Prj.Name));
```

त्रुटि हैंडलिंग के साथ &lt;see cref="LoadOptions" /&gt; का उपयोग करके Primavera प्रोजेक्ट लोड करने का तरीका दर्शाता है।

```csharp
public void WorkWithLoadOptionsAndPrimaveraOptionsAndErrorHandler()
{
    var loadOptions = new LoadOptions();

    var primaveraOptions = new PrimaveraReadOptions
    {
        ProjectUid = 3882
    };

    // Primavera रीडिंग विकल्प सेट करें
    loadOptions.PrimaveraReadOptions = primaveraOptions;
    loadOptions.ErrorHandler = CustomDurationHandlerForFile;

    var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);

    // परियोजना के साथ काम करें...
}

private static object CustomDurationHandlerForFile(object sender, ParseErrorArgs args)
{
    var regex = new Regex("[*]{2}(\\d+)Hrs(\\d+)Mins(\\d+)Secs[*]{2}");
    if (args.FieldType != typeof(TimeSpan))
    {
        throw args.Exception;
    }

    Console.WriteLine("Object field: {0}, Object field type: {1}, Invalid value: {2}", args.FieldName, args.FieldType, args.InvalidValue);
    var duration = regex.Replace(args.InvalidValue, "PT$1H$2M$3S");
    var value = Duration.ParseTimeSpan(duration);
    Console.WriteLine("New value : {0}", value);
    return value;
}
```

### संबंधित देखें

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


