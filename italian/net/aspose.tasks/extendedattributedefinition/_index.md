---
title: Class ExtendedAttributeDefinition
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: Aspose.Tasks.ExtendedAttributeDefinition classe. Rappresenta una definizione di attributo esteso associata a un progetto.
type: docs
weight: 540
url: /it/net/aspose.tasks/extendedattributedefinition/
---
## ExtendedAttributeDefinition class

Rappresenta una definizione di attributo esteso associata a un progetto.

```csharp
public class ExtendedAttributeDefinition
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Alias](../../aspose.tasks/extendedattributedefinition/alias/) { get; set; } | Ottiene o imposta l'alias di un campo personalizzato. |
| [AppendNewValues](../../aspose.tasks/extendedattributedefinition/appendnewvalues/) { get; set; } | Ottiene o imposta un valore che indica se i nuovi valori aggiunti a un progetto vengono aggiunti automaticamente all'elenco. |
| [AutoRollDown](../../aspose.tasks/extendedattributedefinition/autorolldown/) { get; set; } | Ottiene o imposta un valore che indica se è abilitato un rolldown automatico alle assegnazioni. |
| [CalculationType](../../aspose.tasks/extendedattributedefinition/calculationtype/) { get; set; } | Ottiene o imposta il tipo di calcolo del valore dell'attributo personalizzato. |
| [CfType](../../aspose.tasks/extendedattributedefinition/cftype/) { get; } | Ottiene il tipo di un campo personalizzato. |
| [Default](../../aspose.tasks/extendedattributedefinition/default/) { get; set; } | Ottiene o imposta il valore predefinito nell'elenco. |
| [DefaultGuid](../../aspose.tasks/extendedattributedefinition/defaultguid/) { get; set; } | Ottiene o imposta il Guid della voce della tabella di ricerca predefinita. |
| [ElementType](../../aspose.tasks/extendedattributedefinition/elementtype/) { get; set; } | Ottiene o imposta l'attributo esteso associato a un'attività, una risorsa o un'assegnazione. |
| [FieldId](../../aspose.tasks/extendedattributedefinition/fieldid/) { get; set; } | Ottiene o imposta corrisponde all'ID progetto di un campo personalizzato. Usa la rappresentazione di stringa di una costante da[`ExtendedAttributeTask`](../extendedattributetask/) classe da specificare[`FieldId`](./fieldid/) proprietà. |
| [FieldName](../../aspose.tasks/extendedattributedefinition/fieldname/) { get; } | Ottiene il nome di un campo personalizzato. |
| [Formula](../../aspose.tasks/extendedattributedefinition/formula/) { get; set; } | Ottiene o imposta la formula utilizzata da Microsoft Project per popolare un campo attività personalizzato. |
| [Guid](../../aspose.tasks/extendedattributedefinition/guid/) { get; set; } | Ottiene o imposta il Guid di un campo personalizzato. |
| [LookupUid](../../aspose.tasks/extendedattributedefinition/lookupuid/) { get; } | Ottiene un Guid della tabella di ricerca associata a un campo personalizzato. |
| [MaxMultiValues](../../aspose.tasks/extendedattributedefinition/maxmultivalues/) { get; set; } | Ottiene o imposta il numero massimo di valori che è possibile impostare in un elenco di selezione. |
| [ParentProject](../../aspose.tasks/extendedattributedefinition/parentproject/) { get; } | Ottiene il progetto padre per il`ExtendedAttributeDefinition` istanza. |
| [PhoneticsAlias](../../aspose.tasks/extendedattributedefinition/phoneticsalias/) { get; set; } | Ottiene o imposta la pronuncia fonetica dell'alias di un campo personalizzato. |
| [RestrictValues](../../aspose.tasks/extendedattributedefinition/restrictvalues/) { get; set; } | Ottiene o imposta un valore che indica se i valori del campo personalizzato sono limitati ai valori in[`ValueList`](./valuelist/) . |
| [RollupType](../../aspose.tasks/extendedattributedefinition/rolluptype/) { get; set; } | Ottiene o imposta la modalità di calcolo dei rollup. |
| [SecondaryGuid](../../aspose.tasks/extendedattributedefinition/secondaryguid/) { get; set; } | Ottiene o imposta il guid secondario dell'attributo esteso. |
| [SecondaryPid](../../aspose.tasks/extendedattributedefinition/secondarypid/) { get; set; } | Ottiene o imposta il PID secondario di un campo personalizzato. |
| [SummaryRowsCalculationType](../../aspose.tasks/extendedattributedefinition/summaryrowscalculationtype/) { get; set; } | Ottiene o imposta il tipo di calcolo del valore dell'attributo personalizzato per le righe di riepilogo. |
| [UserDef](../../aspose.tasks/extendedattributedefinition/userdef/) { get; set; } | Ottiene o imposta un valore che indica se un campo personalizzato è definito dall'utente. |
| [ValueList](../../aspose.tasks/extendedattributedefinition/valuelist/) { get; } | Ottiene List&lt;Value&gt; ValueList. |
| [ValuelistSortOrder](../../aspose.tasks/extendedattributedefinition/valuelistsortorder/) { get; set; } | Ottiene o imposta il modo in cui vengono ordinate le liste valori. I valori sono: 0=Decrescente, 1=Crescente. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/#createlookupresourcedefinition_1)(ExtendedAttributeResource, string) | Metodo factory che crea una definizione di attributo estesa con lookup. Ha[`CalculationType`](./calculationtype/) uguale aLookup e può essere utilizzato solo in Risorse. È necessario specificare*fieldId* E*alias* quando si chiama questo metodo. Il tipo di campo viene dedotto dal campo id. |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/#createlookupresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Metodo factory che crea una definizione di attributo estesa con lookup. Ha[`CalculationType`](./calculationtype/) uguale aLookup e può essere utilizzato solo in Risorse. È necessario specificare*customFieldType* ,*fieldId* E*alias* quando chiami questo metodo. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/#createlookuptaskdefinition_1)(ExtendedAttributeTask, string) | Metodo factory che crea una definizione di attributo estesa con lookup. Ha[`CalculationType`](./calculationtype/) uguale aLookup e può essere utilizzato solo in Attività. È necessario specificare*fieldId* E*alias* quando si chiama questo metodo. Il tipo di campo viene dedotto dal campo id. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/#createlookuptaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Metodo factory che crea una definizione di attributo estesa con lookup. Ha[`CalculationType`](./calculationtype/) uguale aLookup e può essere utilizzato solo in Attività. È necessario specificare*customFieldType* ,*fieldId* E*alias* quando chiami questo metodo. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition/#createresourcedefinition_1)(ExtendedAttributeResource, string) | Metodo Factory che crea una semplice definizione di attributo esteso, che Microsoft Project mostra come "None". Ha[`CalculationType`](./calculationtype/) uguale aNone e può essere utilizzato solo in Risorsa. È necessario specificare*fieldId* E*alias* quando si chiama questo metodo. Il tipo di campo viene dedotto dal campo id. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition/#createresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Metodo Factory che crea una semplice definizione di attributo esteso, che Microsoft Project mostra come "None". Ha[`CalculationType`](./calculationtype/) uguale aNone e può essere utilizzato solo in Risorsa. È necessario specificare*customFieldType* ,*fieldId* E*alias* quando chiami questo metodo. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition/#createtaskdefinition_1)(ExtendedAttributeTask, string) | Metodo Factory che crea una semplice definizione di attributo esteso, che Microsoft Project mostra come "None". Ha[`CalculationType`](./calculationtype/) uguale aNone e può essere utilizzato solo in Attività. È necessario specificare*fieldId* E*alias* quando si chiama questo metodo. Il tipo di campo viene dedotto da id campo. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition/#createtaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Metodo Factory che crea una semplice definizione di attributo esteso, che Microsoft Project mostra come "None". Ha[`CalculationType`](./calculationtype/) uguale aNone e può essere utilizzato solo in Attività. È necessario specificare*customFieldType* ,*fieldId* E*alias* quando si chiama questo metodo. |
| [AddLookupValue](../../aspose.tasks/extendedattributedefinition/addlookupvalue/)(Value) | Aggiunge un valore all'elenco di ricerca interno. Questo è un modo preferibile per le manipolazioni con il[`ValueList`](./valuelist/) . |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute)() | Crea un nuovo attributo esteso con l'ID campo uguale al valore dell'ID campo di questo oggetto. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_3)(bool) | Crea un nuovo attributo esteso con l'ID campo uguale al valore ID campo di questo oggetto e al valore flag specificato. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_4)(DateTime) | Crea un nuovo attributo esteso con l'ID campo uguale al valore ID campo di questo oggetto e al valore data specificato. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_5)(decimal) | Crea un nuovo attributo esteso con l'ID campo uguale al valore ID campo di questo oggetto e al valore numerico specificato. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_1)(Duration) | Crea un nuovo attributo esteso con l'ID campo uguale al valore dell'ID campo di questo oggetto e al valore di durata specificato. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_6)(string) | Crea un nuovo attributo esteso con l'ID campo uguale al valore ID campo di questo oggetto e al valore di testo specificato. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_2)(Value) | Crea un nuovo attributo esteso collegato a specificato[`Value`](../value/) oggetto. |
| override [Equals](../../aspose.tasks/extendedattributedefinition/equals/)(object) | Restituisce un flag che indica se questa istanza è uguale all'oggetto specificato. |
| override [GetHashCode](../../aspose.tasks/extendedattributedefinition/gethashcode/)() | Restituisce un codice hash per l'istanza di`ExtendedAttributeDefinition` classe. |
| [RemoveLookupValue](../../aspose.tasks/extendedattributedefinition/removelookupvalue/)(Value) | Rimuove un valore dall'elenco di ricerca interno. Questo è un modo preferibile per le manipolazioni con il[`ValueList`](./valuelist/) . |

### Guarda anche

* spazio dei nomi [Aspose.Tasks](../../aspose.tasks/)
* assemblea [Aspose.Tasks](../../)


