---
title: "CustomProjectPropertyCollection.Add"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "CustomProjectPropertyCollection method. एक नई कस्टम property बनाता है"
type: docs
weight: 30
url: /hi/net/aspose.tasks.properties/customprojectpropertycollection/add/
---
## Add(string, string) {#add_3}

एक नया कस्टम प्रॉपर्टी बनाता है।

```csharp
public CustomProjectProperty Add(string name, string value)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | स्ट्रिंग | प्रॉपर्टी का नाम। |
| value | स्ट्रिंग | नव निर्मित property ऑब्जेक्ट का मान। |

### रिटर्न वैल्यू

नव निर्मित property ऑब्जेक्ट।

## उदाहरण

दिखाता है कि कस्टम प्रोजेक्ट प्रॉपर्टी संग्रहों के साथ कैसे काम करें।

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

Console.WriteLine("Is custom properties collection read-only?: " + project.CustomProps.IsReadOnly);

// आइए नई कस्टम प्रॉपर्टीज़ जोड़ें
// संग्रह Boolean, DateTime, Double, String प्रकारों का समर्थन करता है
project.CustomProps.Add("IsEnterprise", true);
project.CustomProps.Add("Project Start Date", new DateTime(2020, 4, 16, 8, 0, 0));
project.CustomProps.Add("Precision", 10d);
project.CustomProps.Add("Custom Name", "MyProject");

// कस्टम प्रॉपर्टीज़ टाइप्ड संग्रह के माध्यम से उपलब्ध हैं
Console.WriteLine("Count of custom properties: " + project.CustomProps.Count);
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
    Console.WriteLine();
}

// कस्टम प्रॉपर्टी मान प्राप्त करें
Console.WriteLine("Custom Name: " + project.CustomProps["Custom Name"]);

// कस्टम प्रॉपर्टीज़ के नामों पर इटरेट करें
foreach (var propsName in project.CustomProps.Names)
{
    Console.WriteLine("Name: " + propsName);
    Console.WriteLine();
}

// एक स्ट्रिंग कुंजी द्वारा मान को हटाया जा सकता है
if (project.CustomProps.Contains("Custom Name"))
{
    project.CustomProps.Remove("Custom Name");
}

// या कोई संग्रह को पूरी तरह से साफ़ कर सकता है
project.CustomProps.Clear();
```

### संबंधित देखें

* class [CustomProjectProperty](../../customprojectproperty/)
* class [CustomProjectPropertyCollection](../)
* namespace [Aspose.Tasks.Properties](../../customprojectpropertycollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string, bool) {#add}

एक नया कस्टम प्रॉपर्टी बनाता है।

```csharp
public CustomProjectProperty Add(string name, bool value)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | स्ट्रिंग | प्रॉपर्टी का नाम। |
| value | Boolean | नव निर्मित property ऑब्जेक्ट का मान। |

### रिटर्न वैल्यू

नव निर्मित property ऑब्जेक्ट।

## उदाहरण

दिखाता है कि कस्टम प्रोजेक्ट प्रॉपर्टी संग्रहों के साथ कैसे काम करें।

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

Console.WriteLine("Is custom properties collection read-only?: " + project.CustomProps.IsReadOnly);

// आइए नई कस्टम प्रॉपर्टीज़ जोड़ें
// संग्रह Boolean, DateTime, Double, String प्रकारों का समर्थन करता है
project.CustomProps.Add("IsEnterprise", true);
project.CustomProps.Add("Project Start Date", new DateTime(2020, 4, 16, 8, 0, 0));
project.CustomProps.Add("Precision", 10d);
project.CustomProps.Add("Custom Name", "MyProject");

// कस्टम प्रॉपर्टीज़ टाइप्ड संग्रह के माध्यम से उपलब्ध हैं
Console.WriteLine("Count of custom properties: " + project.CustomProps.Count);
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
    Console.WriteLine();
}

// कस्टम प्रॉपर्टी मान प्राप्त करें
Console.WriteLine("Custom Name: " + project.CustomProps["Custom Name"]);

// कस्टम प्रॉपर्टीज़ के नामों पर इटरेट करें
foreach (var propsName in project.CustomProps.Names)
{
    Console.WriteLine("Name: " + propsName);
    Console.WriteLine();
}

// एक स्ट्रिंग कुंजी द्वारा मान को हटाया जा सकता है
if (project.CustomProps.Contains("Custom Name"))
{
    project.CustomProps.Remove("Custom Name");
}

// या कोई संग्रह को पूरी तरह से साफ़ कर सकता है
project.CustomProps.Clear();
```

### संबंधित देखें

* class [CustomProjectProperty](../../customprojectproperty/)
* class [CustomProjectPropertyCollection](../)
* namespace [Aspose.Tasks.Properties](../../customprojectpropertycollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string, double) {#add_1}

एक नया कस्टम प्रॉपर्टी बनाता है।

```csharp
public CustomProjectProperty Add(string name, double value)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | स्ट्रिंग | प्रॉपर्टी का नाम। |
| value | Double | नव निर्मित property ऑब्जेक्ट का मान। |

### रिटर्न वैल्यू

नव निर्मित property ऑब्जेक्ट।

## उदाहरण

दिखाता है कि कस्टम प्रोजेक्ट प्रॉपर्टी संग्रहों के साथ कैसे काम करें।

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

Console.WriteLine("Is custom properties collection read-only?: " + project.CustomProps.IsReadOnly);

// आइए नई कस्टम प्रॉपर्टीज़ जोड़ें
// संग्रह Boolean, DateTime, Double, String प्रकारों का समर्थन करता है
project.CustomProps.Add("IsEnterprise", true);
project.CustomProps.Add("Project Start Date", new DateTime(2020, 4, 16, 8, 0, 0));
project.CustomProps.Add("Precision", 10d);
project.CustomProps.Add("Custom Name", "MyProject");

// कस्टम प्रॉपर्टीज़ टाइप्ड संग्रह के माध्यम से उपलब्ध हैं
Console.WriteLine("Count of custom properties: " + project.CustomProps.Count);
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
    Console.WriteLine();
}

// कस्टम प्रॉपर्टी मान प्राप्त करें
Console.WriteLine("Custom Name: " + project.CustomProps["Custom Name"]);

// कस्टम प्रॉपर्टीज़ के नामों पर इटरेट करें
foreach (var propsName in project.CustomProps.Names)
{
    Console.WriteLine("Name: " + propsName);
    Console.WriteLine();
}

// एक स्ट्रिंग कुंजी द्वारा मान को हटाया जा सकता है
if (project.CustomProps.Contains("Custom Name"))
{
    project.CustomProps.Remove("Custom Name");
}

// या कोई संग्रह को पूरी तरह से साफ़ कर सकता है
project.CustomProps.Clear();
```

### संबंधित देखें

* class [CustomProjectProperty](../../customprojectproperty/)
* class [CustomProjectPropertyCollection](../)
* namespace [Aspose.Tasks.Properties](../../customprojectpropertycollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string, DateTime) {#add_2}

एक नया कस्टम प्रॉपर्टी बनाता है।

```csharp
public CustomProjectProperty Add(string name, DateTime value)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | स्ट्रिंग | प्रॉपर्टी का नाम। |
| value | DateTime | नव निर्मित property ऑब्जेक्ट का मान। |

### रिटर्न वैल्यू

नव निर्मित property ऑब्जेक्ट।

## उदाहरण

दिखाता है कि कस्टम प्रोजेक्ट प्रॉपर्टी संग्रहों के साथ कैसे काम करें।

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

Console.WriteLine("Is custom properties collection read-only?: " + project.CustomProps.IsReadOnly);

// आइए नई कस्टम प्रॉपर्टीज़ जोड़ें
// संग्रह Boolean, DateTime, Double, String प्रकारों का समर्थन करता है
project.CustomProps.Add("IsEnterprise", true);
project.CustomProps.Add("Project Start Date", new DateTime(2020, 4, 16, 8, 0, 0));
project.CustomProps.Add("Precision", 10d);
project.CustomProps.Add("Custom Name", "MyProject");

// कस्टम प्रॉपर्टीज़ टाइप्ड संग्रह के माध्यम से उपलब्ध हैं
Console.WriteLine("Count of custom properties: " + project.CustomProps.Count);
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
    Console.WriteLine();
}

// कस्टम प्रॉपर्टी मान प्राप्त करें
Console.WriteLine("Custom Name: " + project.CustomProps["Custom Name"]);

// कस्टम प्रॉपर्टीज़ के नामों पर इटरेट करें
foreach (var propsName in project.CustomProps.Names)
{
    Console.WriteLine("Name: " + propsName);
    Console.WriteLine();
}

// एक स्ट्रिंग कुंजी द्वारा मान को हटाया जा सकता है
if (project.CustomProps.Contains("Custom Name"))
{
    project.CustomProps.Remove("Custom Name");
}

// या कोई संग्रह को पूरी तरह से साफ़ कर सकता है
project.CustomProps.Clear();
```

### संबंधित देखें

* class [CustomProjectProperty](../../customprojectproperty/)
* class [CustomProjectPropertyCollection](../)
* namespace [Aspose.Tasks.Properties](../../customprojectpropertycollection/)
* assembly [Aspose.Tasks](../../../)


