---
title: ExtendedAttributeDefinition.AddLookupValue
second_title: Aspose.Tasks for .NET API Referansı
description: ExtendedAttributeDefinition yöntem. Dahili arama listesine bir değer ekler. Bu manipülasyonlar için tercih edilen bir yoldur.ValueList .
type: docs
weight: 290
url: /tr/net/aspose.tasks/extendedattributedefinition/addlookupvalue/
---
## ExtendedAttributeDefinition.AddLookupValue method

Dahili arama listesine bir değer ekler. Bu, manipülasyonlar için tercih edilen bir yoldur.[`ValueList`](../valuelist/) .

```csharp
public void AddLookupValue(Value value)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| value | Value | Aramaya eklenecek değer. |

### Notlar

Bu yöntem yalnızca şunlar için çalışır:[`ExtendedAttributeDefinition`](../) olan instances [`CalculationType`](../calculationtype/) eşittirLookup .

### Örnekler

Arama listesine yeni Değer eklemek için bu kodu kullanın:

```csharp
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
```

### Ayrıca bakınız

* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* ad alanı [Aspose.Tasks](../../extendedattributedefinition/)
* toplantı [Aspose.Tasks](../../../)


