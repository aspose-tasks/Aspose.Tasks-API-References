---
title: "Classe ExtendedAttributeDefinition"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.ExtendedAttributeDefinition. Rappresenta una definizione di attributo esteso associata a un progetto"
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
| [AutoRollDown](../../aspose.tasks/extendedattributedefinition/autorolldown/) { get; set; } | Ottiene o imposta un valore che indica se è abilitata una propagazione automatica alle assegnazioni. |
| [CalculationType](../../aspose.tasks/extendedattributedefinition/calculationtype/) { get; set; } | Ottiene o imposta il tipo di calcolo del valore dell'attributo personalizzato. |
| [CfType](../../aspose.tasks/extendedattributedefinition/cftype/) { get; } | Ottiene il tipo di un campo personalizzato. |
| [Default](../../aspose.tasks/extendedattributedefinition/default/) { get; set; } | Ottiene o imposta il valore predefinito nell'elenco. |
| [DefaultGuid](../../aspose.tasks/extendedattributedefinition/defaultguid/) { get; set; } | Ottiene o imposta il Guid della voce predefinita della tabella di ricerca. |
| [ElementType](../../aspose.tasks/extendedattributedefinition/elementtype/) { get; set; } | Ottiene o imposta se l'attributo esteso è associato a un task, a una risorsa o a un'assegnazione. |
| [FieldId](../../aspose.tasks/extendedattributedefinition/fieldid/) { get; set; } | Ottiene o imposta il valore che corrisponde all'ID progetto di un campo personalizzato. Usa la rappresentazione stringa di una costante dalla classe [`ExtendedAttributeTask`](../extendedattributetask/) per specificare la proprietà [`FieldId`](./fieldid/). |
| [FieldName](../../aspose.tasks/extendedattributedefinition/fieldname/) { get; } | Ottiene il nome di un campo personalizzato. |
| [Formula](../../aspose.tasks/extendedattributedefinition/formula/) { get; set; } | Ottiene o imposta la formula che Microsoft Project utilizza per popolare un campo attività personalizzato. |
| [GraphicalIndicator](../../aspose.tasks/extendedattributedefinition/graphicalindicator/) { get; set; } | Ottiene o imposta le informazioni degli indicatori grafici associate all'attributo esteso. Applicabile al formato MPP. |
| [Guid](../../aspose.tasks/extendedattributedefinition/guid/) { get; set; } | Ottiene o imposta il GUID di un campo personalizzato. |
| [LookupUid](../../aspose.tasks/extendedattributedefinition/lookupuid/) { get; } | Ottiene il GUID della tabella di ricerca associata a un campo personalizzato. |
| [MaxMultiValues](../../aspose.tasks/extendedattributedefinition/maxmultivalues/) { get; set; } | Ottiene o imposta il numero massimo di valori che è possibile impostare in un elenco a discesa. |
| [ParentProject](../../aspose.tasks/extendedattributedefinition/parentproject/) { get; } | Ottiene il progetto padre per l'istanza `ExtendedAttributeDefinition`. |
| [PhoneticsAlias](../../aspose.tasks/extendedattributedefinition/phoneticsalias/) { get; set; } | Ottiene o imposta la pronuncia fonetica dell'alias di un campo personalizzato. |
| [RestrictValues](../../aspose.tasks/extendedattributedefinition/restrictvalues/) { get; set; } | Ottiene o imposta un valore che indica se i valori del campo personalizzato sono limitati ai valori nella [`ValueList`](./valuelist/). |
| [RollupType](../../aspose.tasks/extendedattributedefinition/rolluptype/) { get; set; } | Ottiene o imposta il modo in cui vengono calcolati i rollup. |
| [SecondaryGuid](../../aspose.tasks/extendedattributedefinition/secondaryguid/) { get; set; } | Ottiene o imposta il GUID secondario dell'attributo esteso. |
| [SecondaryPid](../../aspose.tasks/extendedattributedefinition/secondarypid/) { get; set; } | Ottiene o imposta il PID secondario di un campo personalizzato. |
| [SummaryRowsCalculationType](../../aspose.tasks/extendedattributedefinition/summaryrowscalculationtype/) { get; set; } | Ottiene o imposta il tipo di calcolo del valore dell'attributo personalizzato per le righe di riepilogo. |
| [UserDef](../../aspose.tasks/extendedattributedefinition/userdef/) { get; set; } | Ottiene o imposta un valore che indica se un campo personalizzato è definito dall'utente. |
| [ValueList](../../aspose.tasks/extendedattributedefinition/valuelist/) { get; } | Ottiene la List&lt;Value&gt; ValueList. |
| [ValuelistSortOrder](../../aspose.tasks/extendedattributedefinition/valuelistsortorder/) { get; set; } | Ottiene o imposta il modo in cui le liste di valori sono ordinate. I valori sono: 0=Decrescente, 1=Crescente. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/#createlookupresourcedefinition_1)(ExtendedAttributeResource, string) | Metodo di fabbrica che crea una definizione di attributo esteso con ricerca. Ha [`CalculationType`](./calculationtype/) impostato su Lookup e può essere usato solo nelle Risorse. È necessario specificare *fieldId* e *alias* quando si chiama questo metodo. Il tipo di campo è dedotto dall'ID del campo. |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/#createlookupresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Metodo di fabbrica che crea una definizione di attributo esteso con ricerca. Ha [`CalculationType`](./calculationtype/) impostato su Lookup e può essere usato solo nelle Risorse. È necessario specificare *customFieldType*, *fieldId* e *alias* quando si chiama questo metodo. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/#createlookuptaskdefinition_1)(ExtendedAttributeTask, string) | Metodo di fabbrica che crea una definizione di attributo esteso con ricerca. Ha [`CalculationType`](./calculationtype/) impostato su Lookup e può essere usato solo nelle Attività. È necessario specificare *fieldId* e *alias* quando si chiama questo metodo. Il tipo di campo è dedotto dall'ID del campo. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/#createlookuptaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Metodo di fabbrica che crea una definizione di attributo esteso con ricerca. Ha [`CalculationType`](./calculationtype/) impostato su Lookup e può essere usato solo nelle Attività. È necessario specificare *customFieldType*, *fieldId* e *alias* quando si chiama questo metodo. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition/#createresourcedefinition_1)(ExtendedAttributeResource, string) | Metodo di fabbrica che crea una definizione di attributo esteso semplice, che Microsoft Project mostra come \"None\". Ha [`CalculationType`](./calculationtype/) impostato su None e può essere usato solo nella Risorsa. È necessario specificare *fieldId* e *alias* quando si chiama questo metodo. Il tipo di campo è dedotto dall'ID del campo. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition/#createresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Metodo di fabbrica che crea una definizione di attributo esteso semplice, che Microsoft Project mostra come \"None\". Ha [`CalculationType`](./calculationtype/) impostato su None e può essere usato solo nella Risorsa. È necessario specificare *customFieldType*, *fieldId* e *alias* quando si chiama questo metodo. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition/#createtaskdefinition_1)(ExtendedAttributeTask, string) | Metodo di fabbrica che crea una definizione di attributo esteso semplice, che Microsoft Project mostra come \"None\". Ha [`CalculationType`](./calculationtype/) impostato su None e può essere usato solo nelle Attività. È necessario specificare *fieldId* e *alias* quando si chiama questo metodo. Il tipo di campo è dedotto dall'ID del campo. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition/#createtaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Metodo di fabbrica che crea una definizione di attributo esteso semplice, che Microsoft Project mostra come \"None\". Ha [`CalculationType`](./calculationtype/) impostato su None e può essere usato solo nelle Attività. È necessario specificare *customFieldType*, *fieldId* e *alias* quando si chiama questo metodo. |
| [AddLookupValue](../../aspose.tasks/extendedattributedefinition/addlookupvalue/)(Value) | Aggiunge un valore all'elenco di ricerca interno. Questo è il modo preferito per le manipolazioni con la [`ValueList`](./valuelist/). |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute)() | Crea un nuovo attributo esteso con l'ID campo che è uguale al valore dell'ID campo di questo oggetto. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_3)(bool) | Crea un nuovo attributo esteso con l'ID campo che è uguale al valore dell'ID campo di questo oggetto e al valore della flag specificato. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_4)(DateTime) | Crea un nuovo attributo esteso con l'ID campo che è uguale al valore dell'ID campo di questo oggetto e al valore della data specificato. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_5)(decimal) | Crea un nuovo attributo esteso con l'ID campo che è uguale al valore dell'ID campo di questo oggetto e al valore numerico specificato. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_1)(Duration) | Crea un nuovo attributo esteso con l'ID campo che è uguale al valore dell'ID campo di questo oggetto e al valore della durata specificato. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_6)(string) | Crea un nuovo attributo esteso con l'ID campo che è uguale al valore dell'ID campo di questo oggetto e al valore del testo specificato. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_2)(Value) | Crea un nuovo attributo esteso collegato all'elemento [`Value`](../value/) specificato. |
| override [Equals](../../aspose.tasks/extendedattributedefinition/equals/)(object) | Restituisce una flag che indica se questa istanza è uguale all'oggetto specificato. |
| override [GetHashCode](../../aspose.tasks/extendedattributedefinition/gethashcode/)() | Restituisce un codice hash per l'istanza della classe `ExtendedAttributeDefinition`. |
| [RemoveLookupValue](../../aspose.tasks/extendedattributedefinition/removelookupvalue/)(Value) | Rimuove un valore dall'elenco interno di ricerca. Questo è un modo preferibile per le manipolazioni con il [`ValueList`](./valuelist/). |

## Esempi

Mostra come utilizzare le funzioni matematiche comuni con gli attributi estesi.

```csharp
public static void EvaluateChoose()
{
    var project = CreateTestProjectWithCustomField();

    // Imposta formula
    project.ExtendedAttributes[0].Formula = "Choose(3, \"This is a\", \"right\", \"choice\")";

    // Stampa il valore dell'attributo esteso
    var task = project.RootTask.Children.GetById(1);
    Console.WriteLine(task.ExtendedAttributes[0].TextValue);
}

public static void EvaluateIsNumeric()
{
    string[] numericFormulas =
        {
            "IsNumeric('AAA')", @"IsNUmeric(1)", "IsNumeric(1<0)", "IsNumeric(\"1.1\")", "IsNumeric(Choose((2 + Sgn(2^-3)), 123, \"one two three\"))"
        };

    var project = CreateTestProjectWithCustomField();

    foreach (var numericFormula in numericFormulas)
    {
        // Imposta formula
        project.ExtendedAttributes[0].Formula = numericFormula;

        // Stampa il valore dell'attributo esteso
        var task = project.RootTask.Children.GetById(1);
        Console.WriteLine(task.ExtendedAttributes[0].TextValue);
    }
}

public static void EvaluateSwitch()
{
    var project = CreateTestProjectWithCustomField();

    // Imposta formula
    project.ExtendedAttributes[0].Formula = "Switch( 0 < 1, \"0 is lesser than 1\", 0 > 1, \"0 is greater than 1\")";

    // Stampa il valore dell'attributo esteso
    var task = project.RootTask.Children.GetById(1);
    Console.WriteLine(task.ExtendedAttributes[0].TextValue);
}

public static Project CreateTestProjectWithCustomField()
{
    var project = new Project();
    var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Custom Field");
    project.ExtendedAttributes.Add(definition);

    var task = project.RootTask.Children.Add("Task");

    var attribute = definition.CreateExtendedAttribute();
    task.ExtendedAttributes.Add(attribute);
    return project;
}
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


