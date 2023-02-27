---
title: ExtendedAttributeDefinition.CreateTaskDefinition
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: ExtendedAttributeDefinition metodo. Metodo Factory che crea una semplice definizione di attributo esteso che Microsoft Project mostra come None. HaCalculationType uguale aNone e può essere utilizzato solo in Attività. È necessario specificarecustomFieldType fieldId Ealias quando si chiama questo metodo.
type: docs
weight: 40
url: /it/net/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---
## CreateTaskDefinition(CustomFieldType, ExtendedAttributeTask, string) {#createtaskdefinition}

Metodo Factory che crea una semplice definizione di attributo esteso, che Microsoft Project mostra come "None". Ha[`CalculationType`](../calculationtype/) uguale aNone e può essere utilizzato solo in Attività. È necessario specificare*customFieldType* ,*fieldId* E*alias* quando si chiama questo metodo.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeTask fieldId, string alias)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| customFieldType | CustomFieldType | Il specificato[`CustomFieldType`](../../customfieldtype/) tipo. |
| fieldId | ExtendedAttributeTask | Il specificato[`ExtendedAttributeTask`](../../extendedattributetask/) ID campo. |
| alias | String | Il specificatoString alias. |

### Valore di ritorno

Istanza creata di[`ExtendedAttributeDefinition`](../) classe con specificato*customFieldType* ,*fieldId* E*alias*.

### Esempi

Utilizza questo esempio per creare una definizione di campo di testo personalizzato:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

### Guarda anche

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* spazio dei nomi [Aspose.Tasks](../../extendedattributedefinition/)
* assemblea [Aspose.Tasks](../../../)

---

## CreateTaskDefinition(ExtendedAttributeTask, string) {#createtaskdefinition_1}

Metodo Factory che crea una semplice definizione di attributo esteso, che Microsoft Project mostra come "None". Ha[`CalculationType`](../calculationtype/) uguale aNone e può essere utilizzato solo in Attività. È necessario specificare*fieldId* E*alias* quando si chiama questo metodo. Il tipo di campo viene dedotto da id campo.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(ExtendedAttributeTask fieldId, 
    string alias)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldId | ExtendedAttributeTask | Il specificato[`ExtendedAttributeTask`](../../extendedattributetask/) ID campo. |
| alias | String | Il specificatoString alias. |

### Valore di ritorno

Istanza creata di[`ExtendedAttributeDefinition`](../) classe con specificato*fieldId* E*alias*.

### Esempi

Utilizza questo esempio per creare una definizione di campo di testo personalizzato:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

### Guarda anche

* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* spazio dei nomi [Aspose.Tasks](../../extendedattributedefinition/)
* assemblea [Aspose.Tasks](../../../)


