---
title: ExtendedAttributeDefinition.CreateResourceDefinition
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: ExtendedAttributeDefinition metodo. Metodo Factory che crea una semplice definizione di attributo esteso che Microsoft Project mostra come None. HaCalculationType uguale aNone e può essere utilizzato solo in Risorsa. È necessario specificarecustomFieldType fieldId Ealias quando chiami questo metodo.
type: docs
weight: 30
url: /it/net/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---
## CreateResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createresourcedefinition}

Metodo Factory che crea una semplice definizione di attributo esteso, che Microsoft Project mostra come "None". Ha[`CalculationType`](../calculationtype/) uguale aNone e può essere utilizzato solo in Risorsa. È necessario specificare*customFieldType* ,*fieldId* E*alias* quando chiami questo metodo.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeResource fieldId, string alias)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| customFieldType | CustomFieldType | Il specificato[`CustomFieldType`](../../customfieldtype/) tipo. |
| fieldId | ExtendedAttributeResource | Il specificato[`ExtendedAttributeResource`](../../extendedattributeresource/) ID campo. |
| alias | String | Il specificatoString alias. |

### Valore di ritorno

Istanza creata di[`ExtendedAttributeDefinition`](../) classe con specificato*customFieldType* ,*fieldId* E*alias*.

### Esempi

Utilizza questo esempio per creare una definizione di campo di testo personalizzato:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

### Guarda anche

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* spazio dei nomi [Aspose.Tasks](../../extendedattributedefinition/)
* assemblea [Aspose.Tasks](../../../)

---

## CreateResourceDefinition(ExtendedAttributeResource, string) {#createresourcedefinition_1}

Metodo Factory che crea una semplice definizione di attributo esteso, che Microsoft Project mostra come "None". Ha[`CalculationType`](../calculationtype/) uguale aNone e può essere utilizzato solo in Risorsa. È necessario specificare*fieldId* E*alias* quando si chiama questo metodo. Il tipo di campo viene dedotto dal campo id.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | Il specificato[`ExtendedAttributeResource`](../../extendedattributeresource/) ID campo. |
| alias | String | Il specificatoString alias. |

### Valore di ritorno

Istanza creata di[`ExtendedAttributeDefinition`](../) classe con specificato*fieldId* E*alias*.

### Esempi

Utilizza questo esempio per creare una definizione di campo di testo personalizzato:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

### Guarda anche

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* spazio dei nomi [Aspose.Tasks](../../extendedattributedefinition/)
* assemblea [Aspose.Tasks](../../../)


