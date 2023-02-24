---
title: ExtendedAttributeDefinition.CreateLookupTaskDefinition
second_title: Aspose.Tasks für .NET-API-Referenz
description: ExtendedAttributeDefinition methode. FactoryMethode die eine erweiterte Attributdefinition mit Lookup erstellt. Es hatCalculationType ist gleichLookup und kann nur in Aufgaben verwendet werden. Sie müssen angebenfieldId Undalias beim Aufruf dieser Methode. Der Feldtyp wird aus der FeldID abgeleitet.
type: docs
weight: 20
url: /de/net/aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/
---
## CreateLookupTaskDefinition(ExtendedAttributeTask, string) {#createlookuptaskdefinition_1}

Factory-Methode, die eine erweiterte Attributdefinition mit Lookup erstellt. Es hat[`CalculationType`](../calculationtype/) ist gleichLookup und kann nur in Aufgaben verwendet werden. Sie müssen angeben*fieldId* Und*alias* beim Aufruf dieser Methode. Der Feldtyp wird aus der Feld-ID abgeleitet.

```csharp
public static ExtendedAttributeDefinition CreateLookupTaskDefinition(ExtendedAttributeTask fieldId, 
    string alias)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldId | ExtendedAttributeTask | Die angegebene[`ExtendedAttributeTask`](../../extendedattributetask/) Feld-ID. |
| alias | String | Die angegebeneString alias. |

### Rückgabewert

Erstellte Instanz der[`ExtendedAttributeDefinition`](../) Klasse mit angegeben*fieldId* Und*alias*.

### Beispiele

Verwenden Sie dieses Beispiel, um eine benutzerdefinierte Felddefinition für eine Aufgabe mit Lookup zu erstellen und sie dann mit Textwerten zu füllen:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
taskTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(taskTextAttr);
```

### Siehe auch

* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namensraum [Aspose.Tasks](../../extendedattributedefinition/)
* Montage [Aspose.Tasks](../../../)

---

## CreateLookupTaskDefinition(CustomFieldType, ExtendedAttributeTask, string) {#createlookuptaskdefinition}

Factory-Methode, die eine erweiterte Attributdefinition mit Lookup erstellt. Es hat[`CalculationType`](../calculationtype/) ist gleichLookup und kann nur in Aufgaben verwendet werden. Sie müssen angeben*customFieldType* ,*fieldId* Und*alias* beim Aufruf dieser Methode.

```csharp
public static ExtendedAttributeDefinition CreateLookupTaskDefinition(
    CustomFieldType customFieldType, ExtendedAttributeTask fieldId, string alias)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| customFieldType | CustomFieldType | Die angegebene[`CustomFieldType`](../../customfieldtype/) Typ. |
| fieldId | ExtendedAttributeTask | Die angegebene[`ExtendedAttributeTask`](../../extendedattributetask/) Feld-ID. |
| alias | String | Die angegebeneString alias. |

### Rückgabewert

Erstellte Instanz der[`ExtendedAttributeDefinition`](../) Klasse mit angegeben*customFieldType* ,*fieldId* Und*alias*.

### Beispiele

Verwenden Sie dieses Beispiel, um eine benutzerdefinierte Felddefinition für eine Aufgabe mit Lookup zu erstellen und sie dann mit Textwerten zu füllen:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
taskTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(taskTextAttr);
```

### Siehe auch

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namensraum [Aspose.Tasks](../../extendedattributedefinition/)
* Montage [Aspose.Tasks](../../../)


