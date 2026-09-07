---
title: "क्लास OutlineValueCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.OutlineValueCollection क्लास। OutlineValue ऑब्जेक्ट्स का संग्रह दर्शाता है।"
type: docs
weight: 1220
url: /hi/net/aspose.tasks/outlinevaluecollection/
---
## OutlineValueCollection class

[`OutlineValue`](../outlinevalue/) ऑब्जेक्ट्स का संग्रह दर्शाता है।

```csharp
public class OutlineValueCollection : IList<OutlineValue>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Count](../../aspose.tasks/outlinevaluecollection/count/) { get; } | इस संग्रह में मौजूद तत्वों की संख्या प्राप्त करता है। |
| [IsReadOnly](../../aspose.tasks/outlinevaluecollection/isreadonly/) { get; } | यह दर्शाने वाला मान प्राप्त करता है कि यह संग्रह केवल-पढ़ने योग्य है या नहीं। |
| [Item](../../aspose.tasks/outlinevaluecollection/item/) { get; set; } | निर्दिष्ट सूचकांक पर तत्व को लौटाता है या सेट करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Add](../../aspose.tasks/outlinevaluecollection/add/)(OutlineValue) | निर्दिष्ट आइटम को इस संग्रह में जोड़ता है। |
| [Clear](../../aspose.tasks/outlinevaluecollection/clear/)() | इस संग्रह से सभी आइटम हटाता है। |
| [Contains](../../aspose.tasks/outlinevaluecollection/contains/)(OutlineValue) | यदि निर्दिष्ट आइटम इस संग्रह में पाया जाता है तो true लौटाता है; अन्यथा false। |
| [CopyTo](../../aspose.tasks/outlinevaluecollection/copyto/)(OutlineValue[], int) | निर्दिष्ट एरे सूचकांक से शुरू करके इस संग्रह के तत्वों को निर्दिष्ट एरे में कॉपी करता है। |
| [GetEnumerator](../../aspose.tasks/outlinevaluecollection/getenumerator/)() | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [IndexOf](../../aspose.tasks/outlinevaluecollection/indexof/)(OutlineValue) | इस संग्रह में निर्दिष्ट आइटम का सूचकांक निर्धारित करता है। |
| [Insert](../../aspose.tasks/outlinevaluecollection/insert/)(int, OutlineValue) | निर्दिष्ट सूचकांक पर निर्दिष्ट आइटम डालता है। |
| [Remove](../../aspose.tasks/outlinevaluecollection/remove/)(OutlineValue) | इस संग्रह से विशिष्ट वस्तु की पहली घटना को हटाता है। |
| [RemoveAt](../../aspose.tasks/outlinevaluecollection/removeat/)(int) | निर्दिष्ट सूचकांक पर एक आइटम हटाता है। |

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

* class [OutlineValue](../outlinevalue/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


