---
title: "Aspose::Tasks::ExtendedAttributeDefinition classe"
linktitle: "ExtendedAttributeDefinition"
articleTitle: "ExtendedAttributeDefinition"
second_title: "Aspose.Tasks per C++"
description: "Rappresenta una definizione di attributo esteso associata a un progetto."
type: docs
weight: 10
url: /it/cpp/aspose.tasks/extendedattributedefinition/
---

## ExtendedAttributeDefinition class

Rappresenta una definizione di attributo esteso associata a un progetto.

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddLookupValue](./addlookupvalue/) | Aggiunge un valore all'elenco di ricerca interno. Questo è un modo preferibile per le manipolazioni con il ValueList. |
| [CreateExtendedAttribute (7 overloads)](./createextendedattribute/) | Crea un nuovo attributo esteso con l'ID campo che corrisponde al valore dell'ID campo di questo oggetto. |
| [CreateLookupResourceDefinition (2 overloads)](./createlookupresourcedefinition/) | Metodo di fabbrica che crea una definizione di attributo esteso con lookup. Ha CalculationType uguale a Tasks::CalculationType::Lookup e può essere usato solo in Resources. È necessario specificare customFieldType, fieldId e alias quando si chiama questo metodo. |
| [CreateLookupTaskDefinition (2 overloads)](./createlookuptaskdefinition/) | Metodo di fabbrica che crea una definizione di attributo esteso con lookup. Ha CalculationType uguale a Tasks::CalculationType::Lookup e può essere usato solo in Tasks. È necessario specificare customFieldType, fieldId e alias quando si chiama questo metodo. |
| [CreateResourceDefinition (2 overloads)](./createresourcedefinition/) | Metodo di fabbrica che crea una definizione di attributo esteso semplice, che Microsoft Project mostra come "None". Ha CalculationType uguale a Tasks::CalculationType::None e può essere usato solo in Resource. È necessario specificare customFieldType, fieldId e alias quando si chiama questo metodo. |
| [CreateTaskDefinition (2 overloads)](./createtaskdefinition/) | Metodo di fabbrica che crea una definizione di attributo esteso semplice, che Microsoft Project mostra come "None". Ha CalculationType uguale a Tasks::CalculationType::None e può essere usato solo in Tasks. È necessario specificare customFieldType, fieldId e alias quando si chiama questo metodo. |
| [Equals](./equals/) | Restituisce un flag che indica se questa istanza è uguale all'oggetto specificato. |
| [get_Alias](./get_alias/) | Restituisce l'alias di un campo personalizzato. |
| [get_AppendNewValues](./get_appendnewvalues/) | Restituisce un valore che indica se i nuovi valori aggiunti a un progetto sono aggiunti automaticamente all'elenco. |
| [get_AutoRollDown](./get_autorolldown/) | Restituisce un valore che indica se è abilitato il roll down automatico alle assegnazioni. |
| [get_CalculationType](./get_calculationtype/) | Restituisce il tipo di calcolo del valore dell'attributo personalizzato. |
| [get_CfType](./get_cftype/) | Restituisce il tipo di un campo personalizzato. |
| [get_Default](./get_default/) | Restituisce il valore predefinito nell'elenco. |
| [get_DefaultGuid](./get_defaultguid/) | Restituisce il Guid della voce della tabella di ricerca predefinita. |
| [get_ElementType](./get_elementtype/) | Restituisce l'attributo esteso associato a un'attività, a una risorsa o a un'assegnazione. |
| [get_FieldId](./get_fieldid/) | Restituisce l'identificatore del progetto di un campo personalizzato. Utilizzare la rappresentazione stringa di una costante della classe Aspose::Tasks::ExtendedAttributeTask per specificare la proprietà FieldId. |
| [get_FieldName](./get_fieldname/) | Restituisce il nome di un campo personalizzato. |
| [get_Formula](./get_formula/) | Restituisce la formula che Microsoft Project utilizza per popolare un campo attività personalizzato. |
| [get_GraphicalIndicator](./get_graphicalindicator/) | Restituisce le informazioni degli indicatori grafici associate all'attributo esteso. Applicabile al formato MPP. |
| [get_Guid](./get_guid/) | Restituisce il Guid di un campo personalizzato. |
| [get_LookupUid](./get_lookupuid/) | Restituisce un Guid della tabella di ricerca associata a un campo personalizzato. |
| [get_MaxMultiValues](./get_maxmultivalues/) | Restituisce il numero massimo di valori che è possibile impostare in un elenco a discesa. |
| [get_ParentProject](./get_parentproject/) | Restituisce il progetto padre per l'istanza ExtendedAttributeDefinition. |
| [get_PhoneticsAlias](./get_phoneticsalias/) | Restituisce la pronuncia fonetica dell'alias di un campo personalizzato. |
| [get_RestrictValues](./get_restrictvalues/) | Restituisce un valore che indica se i valori del campo personalizzato sono limitati ai valori nella ValueList. |
| [get_RollupType](./get_rolluptype/) | Restituisce il modo in cui vengono calcolati i rollup. |
| [get_SecondaryGuid](./get_secondaryguid/) | Restituisce il guid secondario dell'attributo esteso. |
| [get_SecondaryPid](./get_secondarypid/) | Restituisce il PID secondario di un campo personalizzato. |
| [get_SummaryRowsCalculationType](./get_summaryrowscalculationtype/) | Restituisce il tipo di calcolo del valore dell'attributo personalizzato per le righe di riepilogo. |
| [get_UserDef](./get_userdef/) | Restituisce un valore che indica se un campo personalizzato è definito dall'utente. |
| [get_ValueList](./get_valuelist/) | Restituisce la List< Value > ValueList. |
| [get_ValuelistSortOrder](./get_valuelistsortorder/) | Restituisce il modo in cui le liste di valori sono ordinate. I valori sono: 0=Discendente, 1=Ascendente. |
| [GetHashCode](./gethashcode/) | Restituisce un codice hash per l'istanza della classe ExtendedAttributeDefinition. |
| [RemoveLookupValue](./removelookupvalue/) | Rimuove un valore dall'elenco di ricerca interno. Questo è un modo preferibile per le manipolazioni con la ValueList. |
| [set_Alias](./set_alias/) | Imposta l'alias di un campo personalizzato. |
| [set_AppendNewValues](./set_appendnewvalues/) | Imposta un valore che indica se i nuovi valori aggiunti a un progetto sono automaticamente aggiunti all'elenco. |
| [set_AutoRollDown](./set_autorolldown/) | Imposta un valore che indica se è abilitato un roll down automatico alle assegnazioni. |
| [set_CalculationType](./set_calculationtype/) | Imposta il tipo di calcolo del valore dell'attributo personalizzato. |
| [set_Default](./set_default/) | Imposta il valore predefinito nell'elenco. |
| [set_DefaultGuid](./set_defaultguid/) | Imposta il Guid della voce predefinita della tabella di ricerca. |
| [set_ElementType](./set_elementtype/) | Imposta l'attributo esteso associato a un'attività, una risorsa o un'assegnazione. |
| [set_FieldId](./set_fieldid/) | Imposta la corrispondenza con l'ID progetto di un campo personalizzato. Usa la rappresentazione stringa di una costante della classe Aspose::Tasks::ExtendedAttributeTask per specificare la proprietà FieldId. |
| [set_Formula](./set_formula/) | Imposta la formula che Microsoft Project utilizza per popolare un campo attività personalizzato. |
| [set_GraphicalIndicator](./set_graphicalindicator/) | Imposta le informazioni degli indicatori grafici associate all'attributo esteso. Applicabile al formato MPP. |
| [set_Guid](./set_guid/) | Imposta il Guid di un campo personalizzato. |
| [set_MaxMultiValues](./set_maxmultivalues/) | Imposta il numero massimo di valori che è possibile impostare in un elenco a discesa. |
| [set_PhoneticsAlias](./set_phoneticsalias/) | Imposta la pronuncia fonetica dell'alias di un campo personalizzato. |
| [set_RestrictValues](./set_restrictvalues/) | Imposta un valore che indica se i valori del campo personalizzato sono limitati ai valori nella ValueList. |
| [set_RollupType](./set_rolluptype/) | Imposta il modo in cui i rollup vengono calcolati. |
| [set_SecondaryGuid](./set_secondaryguid/) | Imposta il guid secondario dell'attributo esteso. |
| [set_SecondaryPid](./set_secondarypid/) | Imposta il PID secondario di un campo personalizzato. |
| [set_SummaryRowsCalculationType](./set_summaryrowscalculationtype/) | Imposta il tipo di calcolo del valore dell'attributo personalizzato per le righe di riepilogo. |
| [set_UserDef](./set_userdef/) | Imposta un valore che indica se un campo personalizzato è definito dall'utente. |
| [set_ValuelistSortOrder](./set_valuelistsortorder/) | Imposta il modo in cui gli elenchi di valori sono ordinati. I valori sono: 0=Discendente, 1=Ascendente. |

