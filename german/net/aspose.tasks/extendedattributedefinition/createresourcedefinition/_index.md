---
title: ExtendedAttributeDefinition.CreateResourceDefinition
second_title: Aspose.Tasks für .NET-API-Referenz
description: ExtendedAttributeDefinition methode. FactoryMethode die eine einfache erweiterte Attributdefinition erstellt die Microsoft Project als None anzeigt. Hat sieCalculationType ist gleichNone und kann nur in Ressource verwendet werden. Sie müssen angebencustomFieldType fieldId Undalias beim Aufruf dieser Methode.
type: docs
weight: 30
url: /de/net/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---
## CreateResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createresourcedefinition}

Factory-Methode, die eine einfache erweiterte Attributdefinition erstellt, die Microsoft Project als "None" anzeigt. Hat sie[`CalculationType`](../calculationtype/) ist gleichNone und kann nur in Ressource verwendet werden. Sie müssen angeben*customFieldType* ,*fieldId* Und*alias* beim Aufruf dieser Methode.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeResource fieldId, string alias)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| customFieldType | CustomFieldType | Die angegebene[`CustomFieldType`](../../customfieldtype/) Typ. |
| fieldId | ExtendedAttributeResource | Die angegebene[`ExtendedAttributeResource`](../../extendedattributeresource/) Feld-ID. |
| alias | String | Die angegebeneString alias. |

### Rückgabewert

Erstellte Instanz der[`ExtendedAttributeDefinition`](../) Klasse mit angegeben*customFieldType* ,*fieldId* Und*alias*.

### Beispiele

Verwenden Sie dieses Beispiel, um eine benutzerdefinierte Textfelddefinition zu erstellen:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

### Siehe auch

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namensraum [Aspose.Tasks](../../extendedattributedefinition/)
* Montage [Aspose.Tasks](../../../)

---

## CreateResourceDefinition(ExtendedAttributeResource, string) {#createresourcedefinition_1}

Factory-Methode, die eine einfache erweiterte Attributdefinition erstellt, die Microsoft Project als "None" anzeigt. Hat sie[`CalculationType`](../calculationtype/) ist gleichNone und kann nur in Ressource verwendet werden. Sie müssen angeben*fieldId* Und*alias* beim Aufruf dieser Methode. Der Feldtyp wird aus der Feld-ID abgeleitet.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | Die angegebene[`ExtendedAttributeResource`](../../extendedattributeresource/) Feld-ID. |
| alias | String | Die angegebeneString alias. |

### Rückgabewert

Erstellte Instanz der[`ExtendedAttributeDefinition`](../) Klasse mit angegeben*fieldId* Und*alias*.

### Beispiele

Verwenden Sie dieses Beispiel, um eine benutzerdefinierte Textfelddefinition zu erstellen:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

### Siehe auch

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namensraum [Aspose.Tasks](../../extendedattributedefinition/)
* Montage [Aspose.Tasks](../../../)


