---
title: "ExtendedAttributeDefinition"
second_title: "Riferimento API di Aspose.Tasks per Python via .NET"
description: 
type: docs
weight: 310
url: /it/python-net/aspose.tasks/extendedattributedefinition/
---

## ExtendedAttributeDefinition class

Rappresenta una definizione di attributo esteso associata a un progetto.

Il tipo ExtendedAttributeDefinition espone i seguenti membri:
## Proprietà
| Nome | Descrizione |
| :- | :- |
| field_id | Ottiene o imposta il valore corrispondente all'ID progetto di un campo personalizzato.<br/>            Utilizza la rappresentazione stringa di una costante dalla classe [ExtendedAttributeTask](/tasks/python-net/aspose.tasks/extendedattributetask/) per specificare la proprietà [field_id](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |
| field_name | Ottiene il nome di un campo personalizzato. |
| cf_type | Ottiene il tipo di un campo personalizzato. |
| guid | Ottiene o imposta il GUID di un campo personalizzato. |
| element_type | Ottiene o imposta l'attributo esteso associato<br/>            a un'attività, a una risorsa o a un'assegnazione. |
| max_multi_values | Ottiene o imposta il numero massimo di valori che è possibile impostare in un elenco a discesa. |
| user_def | Ottiene o imposta un valore che indica se un campo personalizzato è definito dall'utente. |
| alias | Ottiene o imposta l'alias di un campo personalizzato. |
| secondary_pid | Ottiene o imposta il PID secondario di un campo personalizzato. |
| auto_roll_down | Ottiene o imposta un valore che indica se è abilitato il roll down automatico alle assegnazioni. |
| default_guid | Ottiene o imposta il Guid della voce predefinita della tabella di ricerca. |
| lookup_uid | Ottiene un Guid della tabella di ricerca associata a un campo personalizzato. |
| phonetics_alias | Ottiene o imposta la pronuncia fonetica dell'alias di un campo personalizzato. |
| rollup_type | Ottiene o imposta il modo in cui vengono calcolati i rollup. |
| calculation_type | Ottiene o imposta il tipo di calcolo del valore dell'attributo personalizzato. |
| summary_rows_calculation_type | Ottiene o imposta il tipo di calcolo del valore dell'attributo personalizzato per le righe di riepilogo. |
| formula | Ottiene o imposta la formula che Microsoft Project utilizza per popolare un campo attività personalizzato. |
| graphical_indicator | Ottiene o imposta le informazioni degli indicatori grafici associate all'attributo esteso.<br/>            Applicabile al formato MPP. |
| restrict_values | Ottiene o imposta un valore che indica se i valori del campo personalizzato sono limitati ai valori nella [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |
| valuelist_sort_order | Ottiene o imposta il modo in cui le liste di valori sono ordinate. I valori sono: 0=Discendente, 1=Ascendente. |
| append_new_values | Ottiene o imposta un valore che indica se i nuovi valori aggiunti a un progetto sono automaticamente aggiunti alla lista. |
| default | Ottiene o imposta il valore predefinito nella lista. |
| value_list | Ottiene la List<Value> ValueList. |
| secondary_guid | Ottiene o imposta il guid secondario dell'attributo esteso. |
| parent_project | Ottiene il progetto padre per l'istanza di [ExtendedAttributeDefinition](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |
## Methods
| Nome | Descrizione |
| :- | :- |
| create_extended_attribute() | Crea un nuovo attributo esteso con l'ID campo che è uguale al valore dell'ID campo di questo oggetto. |
| create_extended_attribute(text_value) | Crea un nuovo attributo esteso con l'ID campo che è uguale al valore dell'ID campo di questo oggetto e al valore di testo specificato. |
| create_extended_attribute(numeric_value) | Crea un nuovo attributo esteso con l'ID campo che è uguale al valore dell'ID campo di questo oggetto e al valore numerico specificato. |
| create_extended_attribute(date_time_value) | Crea un nuovo attributo esteso con l'ID campo che è uguale al valore dell'ID campo di questo oggetto e al valore di data specificato. |
| create_extended_attribute(duration_value) | Crea un nuovo attributo esteso con l'ID campo che è uguale al valore dell'ID campo di questo oggetto e al valore di durata specificato. |
| create_extended_attribute(flag_value) | Crea un nuovo attributo esteso con l'ID campo che è uguale al valore dell'ID campo di questo oggetto e al valore di flag specificato. |
| create_extended_attribute(lookup_value) | Crea un nuovo attributo esteso collegato all'elemento [Value](/tasks/python-net/aspose.tasks/value/) specificato. |
| create_task_definition(custom_field_type, field_id, alias) | Metodo di fabbrica che crea una semplice definizione di attributo esteso, che Microsoft Project mostra come "None".<br/>            Ha [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) uguale a [NONE](/tasks/python-net/aspose.tasks/calculationtype/) e può essere usato solo nei Task.<br/>            È necessario specificare |
| create_task_definition(field_id, alias) | Metodo di fabbrica che crea una semplice definizione di attributo esteso, che Microsoft Project mostra come "None".<br/>            Ha [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) uguale a [NONE](/tasks/python-net/aspose.tasks/calculationtype/) e può essere usato solo nei Task.<br/>            È necessario specificare |
| create_resource_definition(custom_field_type, field_id, alias) | Metodo di fabbrica che crea una semplice definizione di attributo esteso, che Microsoft Project mostra come "None".<br/>            Ha [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) uguale a [NONE](/tasks/python-net/aspose.tasks/calculationtype/) e può essere usato solo nella Risorsa.<br/>            È necessario specificare |
| create_resource_definition(field_id, alias) | Metodo di fabbrica che crea una semplice definizione di attributo esteso, che Microsoft Project mostra come "None".<br/>            Ha [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) uguale a [NONE](/tasks/python-net/aspose.tasks/calculationtype/) e può essere usato solo nella Risorsa.<br/>            È necessario specificare |
| create_lookup_task_definition(field_id, alias) | Metodo di fabbrica che crea una definizione di attributo esteso con ricerca.<br/>            Ha [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) uguale a [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) e può essere usato solo nei Task.<br/>            È necessario specificare |
| create_lookup_task_definition(custom_field_type, field_id, alias) | Metodo di fabbrica che crea una definizione di attributo esteso con ricerca.<br/>            Ha [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) uguale a [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) e può essere usato solo nei Task.<br/>            È necessario specificare |
| create_lookup_resource_definition(field_id, alias) | Metodo di fabbrica che crea una definizione di attributo esteso con ricerca.<br/>            Ha [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) uguale a [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) e può essere usato solo nelle Risorse.<br/>            È necessario specificare |
| create_lookup_resource_definition(custom_field_type, field_id, alias) | Metodo di fabbrica che crea una definizione di attributo esteso con ricerca.<br/>            Ha [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) uguale a [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) e può essere usato solo nelle Risorse.<br/>            È necessario specificare |
| add_lookup_value(value) | Aggiunge un valore all'elenco interno di ricerca. Questo è il modo consigliato per le manipolazioni con il [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |
| remove_lookup_value(value) | Rimuove un valore dall'elenco interno di ricerca. Questo è il modo consigliato per le manipolazioni con il [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |

### Vedi anche

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

