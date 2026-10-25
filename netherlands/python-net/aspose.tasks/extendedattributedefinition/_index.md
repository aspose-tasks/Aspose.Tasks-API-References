---
title: "ExtendedAttributeDefinition"
second_title: "Aspose.Tasks for Python via .NET API-referentie"
description: 
type: docs
weight: 310
url: /nl/python-net/aspose.tasks/extendedattributedefinition/
---

## ExtendedAttributeDefinition class

Stelt een definitie van een uitgebreid attribuut voor dat aan een project is gekoppeld.

Het type ExtendedAttributeDefinition geeft de volgende leden weer:
## Eigenschappen
| Naam | Beschrijving |
| :- | :- |
| field_id | Haalt op of stelt overeen met de project‑ID van een aangepast veld.<br/>            Gebruik de tekenreeksrepresentatie van een constante uit de [ExtendedAttributeTask](/tasks/python-net/aspose.tasks/extendedattributetask/) klasse om de [field_id](/tasks/python-net/aspose.tasks/extendedattributedefinition/) eigenschap op te geven. |
| field_name | Haalt de naam van een aangepast veld op. |
| cf_type | Haalt het type van een aangepast veld op. |
| guid | Haalt op of stelt de GUID van een aangepast veld in. |
| element_type | Haalt op of stelt in dat het uitgebreide attribuut is gekoppeld<br/>            aan een taak, een resource of een toewijzing. |
| max_multi_values | Haalt op of stelt het maximale aantal waarden in dat u kunt instellen in een keuzelijst. |
| user_def | Haalt op of stelt een waarde in die aangeeft of een aangepast veld door de gebruiker is gedefinieerd. |
| alias | Haalt op of stelt de alias van een aangepast veld in. |
| secondary_pid | Haalt op of stelt de secundaire PID van een aangepast veld in. |
| auto_roll_down | Haalt op of stelt een waarde in die aangeeft of een automatische uitrol naar toewijzingen is ingeschakeld. |
| default_guid | Haalt op of stelt de Guid van de standaard opzoektabelvermelding in. |
| lookup_uid | Haalt een Guid op van de opzoektabel die is gekoppeld aan een aangepast veld. |
| phonetics_alias | Haalt op of stelt de fonetische uitspraak van de alias van een aangepast veld in. |
| rollup_type | Haalt op of stelt de manier waarop roll-ups worden berekend in. |
| calculation_type | Haalt op of stelt het type berekening van de waarde van het aangepaste attribuut in. |
| summary_rows_calculation_type | Haalt op of stelt het type berekening van de waarde van het aangepaste attribuut voor samenvattingsrijen in. |
| formula | Haalt op of stelt de formule in die Microsoft Project gebruikt om een aangepast taakveld te vullen. |
| graphical_indicator | Haalt de grafische indicatorinformatie op of stelt deze in die is gekoppeld aan het uitgebreide attribuut.<br/>            Van toepassing op MPP-indeling. |
| restrict_values | Haalt een waarde op of stelt deze in die aangeeft of de aangepaste veldwaarden beperkt zijn tot waarden in de [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |
| valuelist_sort_order | Haalt de manier op waarop waardelijsten worden gesorteerd of stelt deze in. Waarden zijn: 0=Aflopend, 1=Oplopend. |
| append_new_values | Haalt een waarde op of stelt deze in die aangeeft of nieuwe waarden die aan een project worden toegevoegd automatisch aan de lijst worden toegevoegd. |
| default | Haalt de standaardwaarde in de lijst op of stelt deze in. |
| value_list | Haalt de List<Value> ValueList op. |
| secondary_guid | Haalt de secundaire guid van het uitgebreide attribuut op of stelt deze in. |
| parent_project | Haalt het bovenliggende project op voor de [ExtendedAttributeDefinition](/tasks/python-net/aspose.tasks/extendedattributedefinition/) instantie. |
## Methods
| Naam | Beschrijving |
| :- | :- |
| create_extended_attribute() | Maakt een nieuw uitgebreid attribuut aan met de veld-ID die gelijk is aan de veld-ID-waarde van dit object. |
| create_extended_attribute(text_value) | Maakt een nieuw uitgebreid attribuut aan met de veld-ID die gelijk is aan de veld-ID-waarde van dit object en de opgegeven tekstwaarde. |
| create_extended_attribute(numeric_value) | Maakt een nieuw uitgebreid attribuut aan met de veld-ID die gelijk is aan de veld-ID-waarde van dit object en de opgegeven numerieke waarde. |
| create_extended_attribute(date_time_value) | Maakt een nieuw uitgebreid attribuut aan met de veld-ID die gelijk is aan de veld-ID-waarde van dit object en de opgegeven datumwaarde. |
| create_extended_attribute(duration_value) | Maakt een nieuw uitgebreid attribuut aan met de veld-ID die gelijk is aan de veld-ID-waarde van dit object en de opgegeven duurwaarde. |
| create_extended_attribute(flag_value) | Maakt een nieuw uitgebreid attribuut aan met de veld-ID die gelijk is aan de veld-ID-waarde van dit object en de opgegeven vlagwaarde. |
| create_extended_attribute(lookup_value) | Maakt een nieuw uitgebreid attribuut aan dat gekoppeld is aan het opgegeven [Value](/tasks/python-net/aspose.tasks/value/) item. |
| create_task_definition(custom_field_type, field_id, alias) | Factory-methode die een eenvoudige definitie van een uitgebreid attribuut maakt, die Microsoft Project weergeeft als "None".<br/>            Het heeft [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) gelijk aan [NONE](/tasks/python-net/aspose.tasks/calculationtype/) en kan alleen in Taken worden gebruikt.<br/>            U moet specificeren |
| create_task_definition(field_id, alias) | Factory-methode die een eenvoudige definitie van een uitgebreid attribuut maakt, die Microsoft Project weergeeft als "None".<br/>            Het heeft [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) gelijk aan [NONE](/tasks/python-net/aspose.tasks/calculationtype/) en kan alleen in Taken worden gebruikt.<br/>            U moet specificeren |
| create_resource_definition(custom_field_type, field_id, alias) | Factory-methode die een eenvoudige definitie van een uitgebreid attribuut maakt, die Microsoft Project weergeeft als "None".<br/>            Het heeft [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) gelijk aan [NONE](/tasks/python-net/aspose.tasks/calculationtype/) en kan alleen in Resources worden gebruikt.<br/>            U moet specificeren |
| create_resource_definition(field_id, alias) | Factory-methode die een eenvoudige definitie van een uitgebreid attribuut maakt, die Microsoft Project weergeeft als "None".<br/>            Het heeft [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) gelijk aan [NONE](/tasks/python-net/aspose.tasks/calculationtype/) en kan alleen in Resources worden gebruikt.<br/>            U moet specificeren |
| create_lookup_task_definition(field_id, alias) | Factory-methode die een definitie van een uitgebreid attribuut met opzoeklijst maakt.<br/>            Het heeft [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) gelijk aan [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) en kan alleen in Taken worden gebruikt.<br/>            U moet specificeren |
| create_lookup_task_definition(custom_field_type, field_id, alias) | Factory-methode die een definitie van een uitgebreid attribuut met opzoeklijst maakt.<br/>            Het heeft [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) gelijk aan [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) en kan alleen in Taken worden gebruikt.<br/>            U moet specificeren |
| create_lookup_resource_definition(field_id, alias) | Factory-methode die een definitie van een uitgebreid attribuut met opzoeklijst maakt.<br/>            Het heeft [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) gelijk aan [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) en kan alleen in Resources worden gebruikt.<br/>            U moet specificeren |
| create_lookup_resource_definition(custom_field_type, field_id, alias) | Factory-methode die een definitie van een uitgebreid attribuut met opzoeklijst maakt.<br/>            Het heeft [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) gelijk aan [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) en kan alleen in Resources worden gebruikt.<br/>            U moet specificeren |
| add_lookup_value(value) | Voegt een waarde toe aan de interne opzoeklijst. Dit is de aanbevolen manier om te manipuleren met de [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |
| remove_lookup_value(value) | Verwijdert een waarde uit de interne opzoeklijst. Dit is de aanbevolen manier om te manipuleren met de [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |

### Zie ook

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

