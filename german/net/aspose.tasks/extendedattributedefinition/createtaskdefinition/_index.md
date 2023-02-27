---
title: ExtendedAttributeDefinition.CreateTaskDefinition
second_title: Aspose.Tasks für .NET-API-Referenz
description: ExtendedAttributeDefinition methode. FactoryMethode die eine einfache erweiterte Attributdefinition erstellt die Microsoft Project als None anzeigt. Hat sieCalculationType ist gleichNone und kann nur in Aufgaben verwendet werden. Sie müssen angebencustomFieldType fieldId Undalias beim Aufruf dieser Methode.
type: docs
weight: 40
url: /de/net/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---
## CreateTaskDefinition(CustomFieldType, ExtendedAttributeTask, string) {#createtaskdefinition}

Factory-Methode, die eine einfache erweiterte Attributdefinition erstellt, die Microsoft Project als "None" anzeigt. Hat sie[`CalculationType`](../calculationtype/) ist gleichNone und kann nur in Aufgaben verwendet werden. Sie müssen angeben*customFieldType* ,*fieldId* Und*alias* beim Aufruf dieser Methode.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeTask fieldId, string alias)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| customFieldType | CustomFieldType | Die angegebene[`CustomFieldType`](../../customfieldtype/) Typ. |
| fieldId | ExtendedAttributeTask | Die angegebene[`ExtendedAttributeTask`](../../extendedattributetask/) Feld-ID. |
| alias | String | Die angegebeneString alias. |

### Rückgabewert

Erstellte Instanz der[`ExtendedAttributeDefinition`](../) Klasse mit angegeben*customFieldType* ,*fieldId* Und*alias*.

### Beispiele

Verwenden Sie dieses Beispiel, um eine benutzerdefinierte Textfelddefinition zu erstellen:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

### Siehe auch

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namensraum [Aspose.Tasks](../../extendedattributedefinition/)
* Montage [Aspose.Tasks](../../../)

---

## CreateTaskDefinition(ExtendedAttributeTask, string) {#createtaskdefinition_1}

Factory-Methode, die eine einfache erweiterte Attributdefinition erstellt, die Microsoft Project als "None" anzeigt. Hat sie[`CalculationType`](../calculationtype/) ist gleichNone und kann nur in Aufgaben verwendet werden. Sie müssen angeben*fieldId* Und*alias* beim Aufruf dieser Methode. Der Feldtyp wird aus der Feld-ID abgeleitet.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(ExtendedAttributeTask fieldId, 
    string alias)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldId | ExtendedAttributeTask | Die angegebene[`ExtendedAttributeTask`](../../extendedattributetask/) Feld-ID. |
| alias | String | Die angegebeneString alias. |

### Rückgabewert

Erstellte Instanz der[`ExtendedAttributeDefinition`](../) Klasse mit angegeben*fieldId* Und*alias*.

### Beispiele

Verwenden Sie dieses Beispiel, um eine benutzerdefinierte Textfelddefinition zu erstellen:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

### Siehe auch

* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namensraum [Aspose.Tasks](../../extendedattributedefinition/)
* Montage [Aspose.Tasks](../../../)


