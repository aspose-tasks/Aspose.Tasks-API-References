---
title: ExtendedAttributeDefinition.CreateLookupTaskDefinition
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: ExtendedAttributeDefinition metodo. Metodo factory che crea una definizione di attributo estesa con lookup. HaCalculationType uguale aLookup e può essere utilizzato solo in Attività. È necessario specificarefieldId Ealias quando si chiama questo metodo. Il tipo di campo viene dedotto dal campo id.
type: docs
weight: 20
url: /it/net/aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/
---
## CreateLookupTaskDefinition(ExtendedAttributeTask, string) {#createlookuptaskdefinition_1}

Metodo factory che crea una definizione di attributo estesa con lookup. Ha[`CalculationType`](../calculationtype/) uguale aLookup e può essere utilizzato solo in Attività. È necessario specificare*fieldId* E*alias* quando si chiama questo metodo. Il tipo di campo viene dedotto dal campo id.

```csharp
public static ExtendedAttributeDefinition CreateLookupTaskDefinition(ExtendedAttributeTask fieldId, 
    string alias)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldId | ExtendedAttributeTask | Il specificato[`ExtendedAttributeTask`](../../extendedattributetask/) ID campo. |
| alias | String | Il specificatoString alias. |

### Valore di ritorno

Istanza creata di[`ExtendedAttributeDefinition`](../) classe con specificato*fieldId* E*alias*.

### Esempi

Utilizza questo esempio per creare una definizione di campo personalizzata per un'attività con ricerca e poi riempila con valori di testo:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
taskTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(taskTextAttr);
```

### Guarda anche

* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* spazio dei nomi [Aspose.Tasks](../../extendedattributedefinition/)
* assemblea [Aspose.Tasks](../../../)

---

## CreateLookupTaskDefinition(CustomFieldType, ExtendedAttributeTask, string) {#createlookuptaskdefinition}

Metodo factory che crea una definizione di attributo estesa con lookup. Ha[`CalculationType`](../calculationtype/) uguale aLookup e può essere utilizzato solo in Attività. È necessario specificare*customFieldType* ,*fieldId* E*alias* quando chiami questo metodo.

```csharp
public static ExtendedAttributeDefinition CreateLookupTaskDefinition(
    CustomFieldType customFieldType, ExtendedAttributeTask fieldId, string alias)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| customFieldType | CustomFieldType | Il specificato[`CustomFieldType`](../../customfieldtype/) tipo. |
| fieldId | ExtendedAttributeTask | Il specificato[`ExtendedAttributeTask`](../../extendedattributetask/) ID campo. |
| alias | String | Il specificatoString alias. |

### Valore di ritorno

Istanza creata di[`ExtendedAttributeDefinition`](../) classe con specificato*customFieldType* ,*fieldId* E*alias*.

### Esempi

Utilizza questo esempio per creare una definizione di campo personalizzata per un'attività con ricerca e poi riempila con valori di testo:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
taskTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(taskTextAttr);
```

### Guarda anche

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* spazio dei nomi [Aspose.Tasks](../../extendedattributedefinition/)
* assemblea [Aspose.Tasks](../../../)


