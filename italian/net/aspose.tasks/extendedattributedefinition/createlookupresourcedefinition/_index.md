---
title: ExtendedAttributeDefinition.CreateLookupResourceDefinition
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: ExtendedAttributeDefinition metodo. Metodo factory che crea una definizione di attributo estesa con lookup. HaCalculationType uguale aLookup e può essere utilizzato solo in Risorse. È necessario specificarefieldId Ealias quando si chiama questo metodo. Il tipo di campo viene dedotto dal campo id.
type: docs
weight: 10
url: /it/net/aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/
---
## CreateLookupResourceDefinition(ExtendedAttributeResource, string) {#createlookupresourcedefinition_1}

Metodo factory che crea una definizione di attributo estesa con lookup. Ha[`CalculationType`](../calculationtype/) uguale aLookup e può essere utilizzato solo in Risorse. È necessario specificare*fieldId* E*alias* quando si chiama questo metodo. Il tipo di campo viene dedotto dal campo id.

```csharp
public static ExtendedAttributeDefinition CreateLookupResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | Il specificato[`ExtendedAttributeResource`](../../extendedattributeresource/) ID campo. |
| alias | String | Il specificatoString alias. |

### Valore di ritorno

Istanza creata di[`ExtendedAttributeDefinition`](../) classe con specificato*fieldId* E*alias*.

### Esempi

Utilizza questo esempio per creare una definizione di campo personalizzata per una risorsa con ricerca e poi riempila con valori di testo:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateLookupResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
resourceTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
resourceTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(resourceTextAttr);
```

### Guarda anche

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* spazio dei nomi [Aspose.Tasks](../../extendedattributedefinition/)
* assemblea [Aspose.Tasks](../../../)

---

## CreateLookupResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createlookupresourcedefinition}

Metodo factory che crea una definizione di attributo estesa con lookup. Ha[`CalculationType`](../calculationtype/) uguale aLookup e può essere utilizzato solo in Risorse. È necessario specificare*customFieldType* ,*fieldId* E*alias* quando chiami questo metodo.

```csharp
public static ExtendedAttributeDefinition CreateLookupResourceDefinition(
    CustomFieldType customFieldType, ExtendedAttributeResource fieldId, string alias)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| customFieldType | CustomFieldType | Il specificato[`CustomFieldType`](../../customfieldtype/) tipo. |
| fieldId | ExtendedAttributeResource | Il specificato[`ExtendedAttributeResource`](../../extendedattributeresource/) ID campo. |
| alias | String | Il specificatoString alias. |

### Valore di ritorno

Istanza creata di[`ExtendedAttributeDefinition`](../) classe con specificato*customFieldType* ,*fieldId* E*alias*.

### Esempi

Utilizza questo esempio per creare una definizione di campo personalizzata per una risorsa con ricerca e poi riempila con valori di testo:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateLookupResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
resourceTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
resourceTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(resourceTextAttr);
```

### Guarda anche

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* spazio dei nomi [Aspose.Tasks](../../extendedattributedefinition/)
* assemblea [Aspose.Tasks](../../../)


