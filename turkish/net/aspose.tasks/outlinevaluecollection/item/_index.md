---
title: "OutlineValueCollection.Item"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "OutlineValueCollection özelliği. Belirtilen indeksteki öğeyi döndürür veya ayarlar"
type: docs
weight: 30
url: /tr/net/aspose.tasks/outlinevaluecollection/item/
---
## OutlineValueCollection indexer

Belirtilen indeksteki öğeyi döndürür veya ayarlar.

```csharp
public OutlineValue this[int index] { get; set; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | Alınacak veya ayarlanacak öğenin sıfır tabanlı indeksi. |

### Dönüş Değeri

belirtilen indeksteki öğe.

## Örnekler

Ana hat değer koleksiyonlarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// değer koleksiyonlarını temizle
foreach (var outlineCode in project.OutlineCodes)
{
    // ana hat maskelerini temizle
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

// dizin erişimiyle değeri güncelle
codeDefinition.Values[0].Value = "654321";

// ana hat değerleri üzerinde yineleme yap
foreach (var definitionValue in codeDefinition.Values)
{
    Console.WriteLine("Value: " + definitionValue.Value);
    Console.WriteLine("Value Id: " + definitionValue.ValueId);
    Console.WriteLine("Value Guid: " + definitionValue.ValueGuid);
    Console.WriteLine();
}

// ...
// ana hat değerleriyle çalış
// ...

// gerektiğinde bir değeri kaldır
if (codeDefinition.Values.Contains(value))
{
    codeDefinition.Values.Remove(value);
}

// başlangıç konumuna bir değer ekle
codeDefinition.Values.Insert(0, value);

// eklenen değerin konumunu kontrol et
Console.WriteLine("Index of inserted value: " + codeDefinition.Values.IndexOf(value));

// ...
// ana hat değerleriyle çalış
// ...

// koleksiyondan son değeri kaldır
codeDefinition.Values.RemoveAt(codeDefinition.Values.Count - 1);

// başka bir ana hat kod tanımı oluşturulabilir
var codeDefinition2 = new OutlineCodeDefinition
                          {
                              Alias = "New outline code 2", FieldId = ((int)ExtendedAttributeTask.OutlineCode2).ToString(), FieldName = "Outline Code2"
                          };

// ve ardından ana hat değerlerini kopyala
var outlineValues = new OutlineValue[codeDefinition.Values.Count];
codeDefinition.Values.CopyTo(outlineValues, 0);

foreach (var outlineValue in outlineValues)
{
    codeDefinition2.Values.Add(outlineValue);
}
```

### Ayrıca Bakınız

* class [OutlineValue](../../outlinevalue/)
* class [OutlineValueCollection](../)
* namespace [Aspose.Tasks](../../outlinevaluecollection/)
* assembly [Aspose.Tasks](../../../)


