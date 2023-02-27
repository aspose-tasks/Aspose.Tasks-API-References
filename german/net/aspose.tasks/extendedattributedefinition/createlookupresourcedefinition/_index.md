---
title: ExtendedAttributeDefinition.CreateLookupResourceDefinition
second_title: Aspose.Tasks für .NET-API-Referenz
description: ExtendedAttributeDefinition methode. FactoryMethode die eine erweiterte Attributdefinition mit Lookup erstellt. Es hatCalculationType ist gleichLookup und kann nur in Ressourcen verwendet werden. Sie müssen angebenfieldId Undalias beim Aufruf dieser Methode. Der Feldtyp wird aus der FeldID abgeleitet.
type: docs
weight: 10
url: /de/net/aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/
---
## CreateLookupResourceDefinition(ExtendedAttributeResource, string) {#createlookupresourcedefinition_1}

Factory-Methode, die eine erweiterte Attributdefinition mit Lookup erstellt. Es hat[`CalculationType`](../calculationtype/) ist gleichLookup und kann nur in Ressourcen verwendet werden. Sie müssen angeben*fieldId* Und*alias* beim Aufruf dieser Methode. Der Feldtyp wird aus der Feld-ID abgeleitet.

```csharp
public static ExtendedAttributeDefinition CreateLookupResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | Die angegebene[`ExtendedAttributeResource`](../../extendedattributeresource/) Feld-ID. |
| alias | String | Die angegebeneString alias. |

### Rückgabewert

Erstellte Instanz der[`ExtendedAttributeDefinition`](../) Klasse mit angegeben*fieldId* Und*alias*.

### Beispiele

Verwenden Sie dieses Beispiel, um eine benutzerdefinierte Felddefinition für eine Ressource mit Lookup zu erstellen und sie dann mit Textwerten zu füllen:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateLookupResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
resourceTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
resourceTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(resourceTextAttr);
```

### Siehe auch

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namensraum [Aspose.Tasks](../../extendedattributedefinition/)
* Montage [Aspose.Tasks](../../../)

---

## CreateLookupResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createlookupresourcedefinition}

Factory-Methode, die eine erweiterte Attributdefinition mit Lookup erstellt. Es hat[`CalculationType`](../calculationtype/) ist gleichLookup und kann nur in Ressourcen verwendet werden. Sie müssen angeben*customFieldType* ,*fieldId* Und*alias* beim Aufruf dieser Methode.

```csharp
public static ExtendedAttributeDefinition CreateLookupResourceDefinition(
    CustomFieldType customFieldType, ExtendedAttributeResource fieldId, string alias)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| customFieldType | CustomFieldType | Die angegebene[`CustomFieldType`](../../customfieldtype/) Typ. |
| fieldId | ExtendedAttributeResource | Die angegebene[`ExtendedAttributeResource`](../../extendedattributeresource/) Feld-ID. |
| alias | String | Die angegebeneString alias. |

### Rückgabewert

Erstellte Instanz der[`ExtendedAttributeDefinition`](../) Klasse mit angegeben*customFieldType* ,*fieldId* Und*alias*.

### Beispiele

Verwenden Sie dieses Beispiel, um eine benutzerdefinierte Felddefinition für eine Ressource mit Lookup zu erstellen und sie dann mit Textwerten zu füllen:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateLookupResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
resourceTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
resourceTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(resourceTextAttr);
```

### Siehe auch

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namensraum [Aspose.Tasks](../../extendedattributedefinition/)
* Montage [Aspose.Tasks](../../../)


