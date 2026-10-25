---
title: "OutlineValueCollection.GetEnumerator"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "OutlineValueCollection मेथड। इस संग्रह के लिए एक एनेमरेटर लौटाता है"
type: docs
weight: 80
url: /hi/net/aspose.tasks/outlinevaluecollection/getenumerator/
---
## OutlineValueCollection.GetEnumerator method

इस संग्रह के लिए एक एन्यूमरेटर लौटाता है।

```csharp
public IEnumerator<OutlineValue> GetEnumerator()
```

### रिटर्न वैल्यू

इस संग्रह के लिए एक एनेमरेटर।

## उदाहरण

आउटलाइन वैल्यू संग्रहों के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// वैल्यू संग्रह साफ़ करें
foreach (var outlineCode in project.OutlineCodes)
{
    // आउटलाइन मास्क साफ़ करें
    if (outlineCode.Values.Count <= 0)
    {
        continue;
    }

    if (!outlineCode.Values.IsReadOnly)
    {
        outlineCode.Values.Clear();
    }
}

var codeDefinition = new OutlineCodeDefinition
                         {
                             Alias = "New task outline code1", FieldId = ((int)ExtendedAttributeTask.OutlineCode1).ToString(), FieldName = "Outline Code1"
                         };
var value = new OutlineValue { Description = "Value description", ValueId = 1, Value = "123456", Type = OutlineValueType.Number };
codeDefinition.Values.Add(value);
project.OutlineCodes.Add(codeDefinition);

// सूचकांक पहुँच द्वारा वैल्यू अपडेट करें
codeDefinition.Values[0].Value = "654321";

// आउटलाइन वैल्यूज़ पर इटररेट करें
foreach (var definitionValue in codeDefinition.Values)
{
    Console.WriteLine("Value: " + definitionValue.Value);
    Console.WriteLine("Value Id: " + definitionValue.ValueId);
    Console.WriteLine("Value Guid: " + definitionValue.ValueGuid);
    Console.WriteLine();
}

// ...
// आउटलाइन वैल्यूज़ के साथ काम करें
// ...

// ज़रूरत पड़ने पर वैल्यू हटाएँ
if (codeDefinition.Values.Contains(value))
{
    codeDefinition.Values.Remove(value);
}

// शुरुआती स्थिति में वैल्यू डालें
codeDefinition.Values.Insert(0, value);

// डाली गई वैल्यू की स्थिति जाँचें
Console.WriteLine("Index of inserted value: " + codeDefinition.Values.IndexOf(value));

// ...
// आउटलाइन वैल्यूज़ के साथ काम करें
// ...

// संग्रह से अंतिम वैल्यू हटाएँ
codeDefinition.Values.RemoveAt(codeDefinition.Values.Count - 1);

// एक और आउटलाइन कोड परिभाषा बनाई जा सकती है
var codeDefinition2 = new OutlineCodeDefinition
                          {
                              Alias = "New outline code 2", FieldId = ((int)ExtendedAttributeTask.OutlineCode2).ToString(), FieldName = "Outline Code2"
                          };

// और फिर आउटलाइन वैल्यूज़ कॉपी करें
var outlineValues = new OutlineValue[codeDefinition.Values.Count];
codeDefinition.Values.CopyTo(outlineValues, 0);

foreach (var outlineValue in outlineValues)
{
    codeDefinition2.Values.Add(outlineValue);
}
```

### संबंधित देखें

* class [OutlineValue](../../outlinevalue/)
* class [OutlineValueCollection](../)
* namespace [Aspose.Tasks](../../outlinevaluecollection/)
* assembly [Aspose.Tasks](../../../)


