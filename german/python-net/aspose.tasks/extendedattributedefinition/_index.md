---
title: "ExtendedAttributeDefinition"
second_title: "Aspose.Tasks für Python via .NET API-Referenz"
description: 
type: docs
weight: 310
url: /de/python-net/aspose.tasks/extendedattributedefinition/
---

## ExtendedAttributeDefinition class

Stellt eine erweiterte Attributdefinition dar, die mit einem Projekt verknüpft ist.

Der Typ ExtendedAttributeDefinition stellt die folgenden Member bereit:
## Eigenschaften
| Name | Beschreibung |
| :- | :- |
| field_id | Liest oder setzt die Projekt-ID eines benutzerdefinierten Feldes.<br/>            Verwenden Sie die Zeichenkettenrepräsentation einer Konstanten aus der Klasse [ExtendedAttributeTask](/tasks/python-net/aspose.tasks/extendedattributetask/) , um die Eigenschaft [field_id](/tasks/python-net/aspose.tasks/extendedattributedefinition/) festzulegen. |
| field_name | Liest den Namen eines benutzerdefinierten Feldes. |
| cf_type | Liest den Typ eines benutzerdefinierten Feldes. |
| guid | Liest oder setzt die GUID eines benutzerdefinierten Feldes. |
| element_type | Liest oder setzt, ob das erweiterte Attribut zugeordnet ist<br/>            zu einem Vorgang, einer Ressource oder einer Zuordnung. |
| max_multi_values | Liest oder setzt die maximale Anzahl von Werten, die Sie in einer Auswahlliste festlegen können. |
| user_def | Liest oder setzt einen Wert, der angibt, ob ein benutzerdefiniertes Feld vom Benutzer definiert ist. |
| alias | Liest oder setzt den Alias eines benutzerdefinierten Feldes. |
| secondary_pid | Liest oder setzt die sekundäre PID eines benutzerdefinierten Feldes. |
| auto_roll_down | Liest oder setzt einen Wert, der angibt, ob ein automatisches Herunterrollen zu Zuweisungen aktiviert ist. |
| default_guid | Liest oder setzt die GUID des Standard-Lookup-Tabelleneintrags. |
| lookup_uid | Liest eine GUID der Lookup-Tabelle, die einem benutzerdefinierten Feld zugeordnet ist. |
| phonetics_alias | Liest oder setzt die phonetische Aussprache des Alias eines benutzerdefinierten Feldes. |
| rollup_type | Liest oder setzt die Art und Weise, wie Rollups berechnet werden. |
| calculation_type | Liest oder setzt den Berechnungstyp des Werts des benutzerdefinierten Attributs. |
| summary_rows_calculation_type | Liest oder setzt den Berechnungstyp des Werts des benutzerdefinierten Attributs für Zusammenfassungszeilen. |
| formula | Liest oder setzt die Formel, die Microsoft Project verwendet, um ein benutzerdefiniertes Aufgabefeld zu füllen. |
| graphical_indicator | Liest oder setzt grafische Indikatorinformationen, die dem erweiterten Attribut zugeordnet sind.<br/>            Anwendbar auf das MPP-Format. |
| restrict_values | Liest oder setzt einen Wert, der angibt, ob die benutzerdefinierten Feldwerte auf Werte in der [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/) beschränkt sind. |
| valuelist_sort_order | Liest oder setzt die Sortierreihenfolge von Wertlisten. Werte sind: 0=Absteigend, 1=Aufsteigend. |
| append_new_values | Liest oder setzt einen Wert, der angibt, ob neue, zu einem Projekt hinzugefügte Werte automatisch zur Liste hinzugefügt werden. |
| default | Liest oder setzt den Standardwert in der Liste. |
| value_list | Liest die List<Value> ValueList. |
| secondary_guid | Liest oder setzt die sekundäre GUID des erweiterten Attributs. |
| parent_project | Liest das übergeordnete Projekt für die [ExtendedAttributeDefinition](/tasks/python-net/aspose.tasks/extendedattributedefinition/) Instanz. |
## Methoden
| Name | Beschreibung |
| :- | :- |
| create_extended_attribute() | Erstellt ein neues erweitertes Attribut mit der Feld-ID, die dem Feld-ID-Wert dieses Objekts entspricht. |
| create_extended_attribute(text_value) | Erstellt ein neues erweitertes Attribut mit der Feld-ID, die dem Feld-ID-Wert dieses Objekts entspricht, und dem angegebenen Textwert. |
| create_extended_attribute(numeric_value) | Erstellt ein neues erweitertes Attribut mit der Feld-ID, die dem Feld-ID-Wert dieses Objekts entspricht, und dem angegebenen numerischen Wert. |
| create_extended_attribute(date_time_value) | Erstellt ein neues erweitertes Attribut mit der Feld-ID, die dem Feld-ID-Wert dieses Objekts entspricht, und dem angegebenen Datumswert. |
| create_extended_attribute(duration_value) | Erstellt ein neues erweitertes Attribut mit der Feld-ID, die dem Feld-ID-Wert dieses Objekts entspricht, und dem angegebenen Dauernwert. |
| create_extended_attribute(flag_value) | Erstellt ein neues erweitertes Attribut mit der Feld-ID, die dem Feld-ID-Wert dieses Objekts entspricht, und dem angegebenen Flag-Wert. |
| create_extended_attribute(lookup_value) | Erstellt ein neues erweitertes Attribut, das mit dem angegebenen [Value](/tasks/python-net/aspose.tasks/value/) Element verknüpft ist. |
| create_task_definition(custom_field_type, field_id, alias) | Factory-Methode, die eine einfache erweiterte Attributdefinition erstellt, die Microsoft Project als "None" anzeigt.<br/>            Sie hat [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) gleich [NONE](/tasks/python-net/aspose.tasks/calculationtype/) und kann nur in Aufgaben verwendet werden.<br/>            Sie müssen angeben |
| create_task_definition(field_id, alias) | Factory-Methode, die eine einfache erweiterte Attributdefinition erstellt, die Microsoft Project als "None" anzeigt.<br/>            Sie hat [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) gleich [NONE](/tasks/python-net/aspose.tasks/calculationtype/) und kann nur in Aufgaben verwendet werden.<br/>            Sie müssen angeben |
| create_resource_definition(custom_field_type, field_id, alias) | Factory-Methode, die eine einfache erweiterte Attributdefinition erstellt, die Microsoft Project als "None" anzeigt.<br/>            Sie hat [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) gleich [NONE](/tasks/python-net/aspose.tasks/calculationtype/) und kann nur in Ressourcen verwendet werden.<br/>            Sie müssen angeben |
| create_resource_definition(field_id, alias) | Factory-Methode, die eine einfache erweiterte Attributdefinition erstellt, die Microsoft Project als "None" anzeigt.<br/>            Sie hat [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) gleich [NONE](/tasks/python-net/aspose.tasks/calculationtype/) und kann nur in Ressourcen verwendet werden.<br/>            Sie müssen angeben |
| create_lookup_task_definition(field_id, alias) | Factory-Methode, die eine erweiterte Attributdefinition mit Lookup erstellt.<br/>            Sie hat [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) gleich [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) und kann nur in Aufgaben verwendet werden.<br/>            Sie müssen angeben |
| create_lookup_task_definition(custom_field_type, field_id, alias) | Factory-Methode, die eine erweiterte Attributdefinition mit Lookup erstellt.<br/>            Sie hat [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) gleich [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) und kann nur in Aufgaben verwendet werden.<br/>            Sie müssen angeben |
| create_lookup_resource_definition(field_id, alias) | Factory-Methode, die eine erweiterte Attributdefinition mit Lookup erstellt.<br/>            Sie hat [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) gleich [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) und kann nur in Ressourcen verwendet werden.<br/>            Sie müssen angeben |
| create_lookup_resource_definition(custom_field_type, field_id, alias) | Factory-Methode, die eine erweiterte Attributdefinition mit Lookup erstellt.<br/>            Sie hat [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) gleich [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) und kann nur in Ressourcen verwendet werden.<br/>            Sie müssen angeben |
| add_lookup_value(value) | Fügt einen Wert zur internen Lookup-Liste hinzu. Dies ist ein bevorzugter Weg für Manipulationen mit der [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |
| remove_lookup_value(value) | Entfernt einen Wert aus der internen Lookup-Liste. Dies ist ein bevorzugter Weg für Manipulationen mit der [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |

### Siehe auch

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

