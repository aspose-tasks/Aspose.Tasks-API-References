---
title: ExtendedAttributeDefinition.AddLookupValue
second_title: Aspose.Tasks für .NET-API-Referenz
description: ExtendedAttributeDefinition methode. Fügt der internen Nachschlageliste einen Wert hinzu. Dies ist ein bevorzugter Weg für Manipulationen mit demValueList .
type: docs
weight: 290
url: /de/net/aspose.tasks/extendedattributedefinition/addlookupvalue/
---
## ExtendedAttributeDefinition.AddLookupValue method

Fügt der internen Nachschlageliste einen Wert hinzu. Dies ist ein bevorzugter Weg für Manipulationen mit dem[`ValueList`](../valuelist/) .

```csharp
public void AddLookupValue(Value value)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | Value | Wert, der der Suche hinzugefügt werden soll. |

### Bemerkungen

Diese Methode funktioniert nur für[`ExtendedAttributeDefinition`](../) instances welche haben[`CalculationType`](../calculationtype/) ist gleichLookup .

### Beispiele

Verwenden Sie diesen Code, um einen neuen Wert zur Suchliste hinzuzufügen:

```csharp
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
```

### Siehe auch

* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* namensraum [Aspose.Tasks](../../extendedattributedefinition/)
* Montage [Aspose.Tasks](../../../)


