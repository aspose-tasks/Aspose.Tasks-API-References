---
title: "ExtendedAttributeDefinition"
second_title: "Aspose.Tasks för Python via .NET API-referens"
description: 
type: docs
weight: 310
url: /sv/python-net/aspose.tasks/extendedattributedefinition/
---

## ExtendedAttributeDefinition class

Representerar en definition av ett utökat attribut som är associerat med ett projekt.

ExtendedAttributeDefinition-typen exponerar följande medlemmar:
## Egenskaper
| Namn | Beskrivning |
| :- | :- |
| field_id | Hämtar eller anger motsvarar projekt‑id för ett anpassat fält.<br/>            Använd strängrepresentationen av en konstant från klassen [ExtendedAttributeTask](/tasks/python-net/aspose.tasks/extendedattributetask/) för att ange egenskapen [field_id](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |
| field_name | Hämtar namnet på ett anpassat fält. |
| cf_type | Hämtar typen av ett anpassat fält. |
| guid | Hämtar eller anger GUID för ett anpassat fält. |
| element_type | Hämtar eller anger att det utökade attributet är associerat<br/>            med en uppgift, en resurs eller en tilldelning. |
| max_multi_values | Hämtar eller anger det maximala antalet värden du kan ange i en urvalslista. |
| user_def | Hämtar eller anger ett värde som visar om ett anpassat fält är användardefinierat. |
| alias | Hämtar eller anger aliaset för ett anpassat fält. |
| secondary_pid | Hämtar eller anger den sekundära PID:n för ett anpassat fält. |
| auto_roll_down | Hämtar eller anger ett värde som visar om en automatisk nedrullning till tilldelningar är aktiverad. |
| default_guid | Hämtar eller anger GUID för standardposten i uppslagstabellen. |
| lookup_uid | Hämtar en GUID för uppslagstabellen som är associerad med ett anpassat fält. |
| phonetics_alias | Hämtar eller anger den fonetiska uttalningen av aliaset för ett anpassat fält. |
| rollup_type | Hämtar eller anger hur sammanslagningar beräknas. |
| calculation_type | Hämtar eller anger typen av beräkning för det anpassade attributets värde. |
| summary_rows_calculation_type | Hämtar eller anger typen av beräkning för det anpassade attributets värde för sammanfattningsrader. |
| formula | Hämtar eller anger formeln som Microsoft Project använder för att fylla i ett anpassat uppgiftsfält. |
| graphical_indicator | Hämtar eller anger information om grafiska indikatorer som är associerad med det utökade attributet.<br/>            Gäller för MPP-format. |
| restrict_values | Hämtar eller anger ett värde som indikerar om de anpassade fältvärdena är begränsade till värden i [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |
| valuelist_sort_order | Hämtar eller anger hur värdelistor sorteras. Värden är: 0=Fallande, 1=Stigande. |
| append_new_values | Hämtar eller anger ett värde som indikerar om nya värden som läggs till i ett projekt automatiskt läggs till i listan. |
| default | Hämtar eller anger standardvärdet i listan. |
| value_list | Hämtar List<Value> ValueList. |
| secondary_guid | Hämtar eller anger den sekundära guid för det utökade attributet. |
| parent_project | Hämtar föräldraprojektet för [ExtendedAttributeDefinition](/tasks/python-net/aspose.tasks/extendedattributedefinition/)-instansen. |
## Methods
| Namn | Beskrivning |
| :- | :- |
| create_extended_attribute() | Skapar ett nytt utökat attribut med fält‑ID som är lika med detta objekts fält‑ID‑värde. |
| create_extended_attribute(text_value) | Skapar ett nytt utökat attribut med fält‑ID som är lika med detta objekts fält‑ID‑värde och det angivna textvärdet. |
| create_extended_attribute(numeric_value) | Skapar ett nytt utökat attribut med fält‑ID som är lika med detta objekts fält‑ID‑värde och det angivna numeriska värdet. |
| create_extended_attribute(date_time_value) | Skapar ett nytt utökat attribut med fält‑ID som är lika med detta objekts fält‑ID‑värde och det angivna datumvärdet. |
| create_extended_attribute(duration_value) | Skapar ett nytt utökat attribut med fält‑ID som är lika med detta objekts fält‑ID‑värde och det angivna varaktighetsvärdet. |
| create_extended_attribute(flag_value) | Skapar ett nytt utökat attribut med fält‑ID som är lika med detta objekts fält‑ID‑värde och det angivna flaggvärdet. |
| create_extended_attribute(lookup_value) | Skapar ett nytt utökat attribut länkat till det angivna [Value](/tasks/python-net/aspose.tasks/value/)‑objektet. |
| create_task_definition(custom_field_type, field_id, alias) | Fabrikmetod som skapar en enkel definition av utökat attribut, som Microsoft Project visar som \"None\".<br/>            Den har [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) lika med [NONE](/tasks/python-net/aspose.tasks/calculationtype/) och kan endast användas i Tasks.<br/>            Du måste ange |
| create_task_definition(field_id, alias) | Fabrikmetod som skapar en enkel definition av utökat attribut, som Microsoft Project visar som \"None\".<br/>            Den har [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) lika med [NONE](/tasks/python-net/aspose.tasks/calculationtype/) och kan endast användas i Tasks.<br/>            Du måste ange |
| create_resource_definition(custom_field_type, field_id, alias) | Fabrikmetod som skapar en enkel definition av utökat attribut, som Microsoft Project visar som \"None\".<br/>            Den har [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) lika med [NONE](/tasks/python-net/aspose.tasks/calculationtype/) och kan endast användas i Resource.<br/>            Du måste ange |
| create_resource_definition(field_id, alias) | Fabrikmetod som skapar en enkel definition av utökat attribut, som Microsoft Project visar som \"None\".<br/>            Den har [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) lika med [NONE](/tasks/python-net/aspose.tasks/calculationtype/) och kan endast användas i Resource.<br/>            Du måste ange |
| create_lookup_task_definition(field_id, alias) | Fabrikmetod som skapar en definition av utökat attribut med uppslagning.<br/>            Den har [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) lika med [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) och kan endast användas i Tasks.<br/>            Du måste ange |
| create_lookup_task_definition(custom_field_type, field_id, alias) | Fabrikmetod som skapar en definition av utökat attribut med uppslagning.<br/>            Den har [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) lika med [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) och kan endast användas i Tasks.<br/>            Du måste ange |
| create_lookup_resource_definition(field_id, alias) | Fabrikmetod som skapar en definition av utökat attribut med uppslagning.<br/>            Den har [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) lika med [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) och kan endast användas i Resources.<br/>            Du måste ange |
| create_lookup_resource_definition(custom_field_type, field_id, alias) | Fabrikmetod som skapar en definition av utökat attribut med uppslagning.<br/>            Den har [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) lika med [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) och kan endast användas i Resources.<br/>            Du måste ange |
| add_lookup_value(value) | Lägger till ett värde i den interna uppslagslistan. Detta är ett föredraget sätt att manipulera [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |
| remove_lookup_value(value) | Tar bort ett värde från den interna uppslagslistan. Detta är ett föredraget sätt att manipulera [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |

### Se även

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

