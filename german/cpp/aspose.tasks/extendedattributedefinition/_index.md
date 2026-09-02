---
title: "Aspose::Tasks::ExtendedAttributeDefinition class"
linktitle: "ExtendedAttributeDefinition"
articleTitle: "ExtendedAttributeDefinition"
second_title: "Aspose.Tasks für C++"
description: "Stellt eine erweiterte Attributdefinition dar, die mit einem Projekt verknüpft ist."
type: docs
weight: 10
url: /de/cpp/aspose.tasks/extendedattributedefinition/
---

## ExtendedAttributeDefinition class

Stellt eine erweiterte Attributdefinition dar, die mit einem Projekt verknüpft ist.

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AddLookupValue](./addlookupvalue/) | Fügt einen Wert zur internen Lookup-Liste hinzu. Dies ist ein bevorzugter Weg für Manipulationen mit der ValueList . |
| [CreateExtendedAttribute (7 overloads)](./createextendedattribute/) | Erstellt ein neues erweitertes Attribut mit der Feld-ID, die dem Feld-ID-Wert dieses Objekts entspricht. |
| [CreateLookupResourceDefinition (2 overloads)](./createlookupresourcedefinition/) | Factory-Methode, die eine erweiterte Attributdefinition mit Lookup erstellt. Sie hat CalculationType gleich zu Tasks::CalculationType::Lookup und kann nur in Resources verwendet werden. Sie müssen customFieldType , fieldId und alias angeben, wenn Sie diese Methode aufrufen. |
| [CreateLookupTaskDefinition (2 overloads)](./createlookuptaskdefinition/) | Factory-Methode, die eine erweiterte Attributdefinition mit Lookup erstellt. Sie hat CalculationType gleich zu Tasks::CalculationType::Lookup und kann nur in Tasks verwendet werden. Sie müssen customFieldType , fieldId und alias angeben, wenn Sie diese Methode aufrufen. |
| [CreateResourceDefinition (2 overloads)](./createresourcedefinition/) | Factory-Methode, die eine einfache erweiterte Attributdefinition erstellt, die Microsoft Project als "None" anzeigt. Sie hat CalculationType gleich zu Tasks::CalculationType::None und kann nur in Resource verwendet werden. Sie müssen customFieldType , fieldId und alias angeben, wenn Sie diese Methode aufrufen. |
| [CreateTaskDefinition (2 overloads)](./createtaskdefinition/) | Factory-Methode, die eine einfache erweiterte Attributdefinition erstellt, die Microsoft Project als "None" anzeigt. Sie hat CalculationType gleich zu Tasks::CalculationType::None und kann nur in Tasks verwendet werden. Sie müssen customFieldType , fieldId und alias angeben, wenn Sie diese Methode aufrufen. |
| [Equals](./equals/) | Gibt ein Flag zurück, das angibt, ob diese Instanz dem angegebenen Objekt gleich ist. |
| [get_Alias](./get_alias/) | Ruft den Alias eines benutzerdefinierten Feldes ab. |
| [get_AppendNewValues](./get_appendnewvalues/) | Ruft einen Wert ab, der angibt, ob neue zu einem Projekt hinzugefügte Werte automatisch zur Liste hinzugefügt werden. |
| [get_AutoRollDown](./get_autorolldown/) | Ruft einen Wert ab, der angibt, ob ein automatisches Herunterrollen zu Zuweisungen aktiviert ist. |
| [get_CalculationType](./get_calculationtype/) | Ruft den Berechnungstyp des Werts des benutzerdefinierten Attributs ab. |
| [get_CfType](./get_cftype/) | Ruft den Typ eines benutzerdefinierten Feldes ab. |
| [get_Default](./get_default/) | Ruft den Standardwert in der Liste ab. |
| [get_DefaultGuid](./get_defaultguid/) | Ruft die Guid des Standard-Lookup-Tabelleneintrags ab. |
| [get_ElementType](./get_elementtype/) | Ruft ab, dass das erweiterte Attribut mit einer Aufgabe, einer Ressource oder einer Zuweisung verknüpft ist. |
| [get_FieldId](./get_fieldid/) | Ruft die Projekt-ID eines benutzerdefinierten Feldes ab. Verwenden Sie die Zeichenkettenrepräsentation einer Konstanten aus der Klasse Aspose::Tasks::ExtendedAttributeTask, um die Eigenschaft FieldId anzugeben. |
| [get_FieldName](./get_fieldname/) | Ruft den Namen eines benutzerdefinierten Feldes ab. |
| [get_Formula](./get_formula/) | Ruft die Formel ab, die Microsoft Project verwendet, um ein benutzerdefiniertes Aufgabefeld zu füllen. |
| [get_GraphicalIndicator](./get_graphicalindicator/) | Ruft grafische Indikatorinformationen ab, die dem erweiterten Attribut zugeordnet sind. Gilt für das MPP-Format. |
| [get_Guid](./get_guid/) | Ruft die Guid eines benutzerdefinierten Feldes ab. |
| [get_LookupUid](./get_lookupuid/) | Ruft die Guid der Lookup-Tabelle ab, die einem benutzerdefinierten Feld zugeordnet ist. |
| [get_MaxMultiValues](./get_maxmultivalues/) | Ruft die maximale Anzahl von Werten ab, die Sie in einer Auswahlliste festlegen können. |
| [get_ParentProject](./get_parentproject/) | Ruft das übergeordnete Projekt für die Instanz ExtendedAttributeDefinition ab. |
| [get_PhoneticsAlias](./get_phoneticsalias/) | Ruft die phonetische Aussprache des Alias eines benutzerdefinierten Feldes ab. |
| [get_RestrictValues](./get_restrictvalues/) | Ruft einen Wert ab, der angibt, ob die Werte des benutzerdefinierten Feldes auf die Werte in der ValueList beschränkt sind. |
| [get_RollupType](./get_rolluptype/) | Ruft die Art der Berechnung von Rollups ab. |
| [get_SecondaryGuid](./get_secondaryguid/) | Ruft die sekundäre Guid des erweiterten Attributs ab. |
| [get_SecondaryPid](./get_secondarypid/) | Ruft die sekundäre PID eines benutzerdefinierten Feldes ab. |
| [get_SummaryRowsCalculationType](./get_summaryrowscalculationtype/) | Ruft den Berechnungstyp des Werts des benutzerdefinierten Attributs für Zusammenfassungszeilen ab. |
| [get_UserDef](./get_userdef/) | Ruft einen Wert ab, der angibt, ob ein benutzerdefiniertes Feld vom Benutzer definiert ist. |
| [get_ValueList](./get_valuelist/) | Ruft die List< Value > ValueList ab. |
| [get_ValuelistSortOrder](./get_valuelistsortorder/) | Ruft die Art der Sortierung von Wertlisten ab. Werte sind: 0=Absteigend, 1=Aufsteigend. |
| [GetHashCode](./gethashcode/) | Gibt einen Hashcode für die Instanz der Klasse ExtendedAttributeDefinition zurück. |
| [RemoveLookupValue](./removelookupvalue/) | Entfernt einen Wert aus der internen Lookup-Liste. Dies ist ein bevorzugter Weg für Manipulationen mit der ValueList. |
| [set_Alias](./set_alias/) | Legt den Alias eines benutzerdefinierten Feldes fest. |
| [set_AppendNewValues](./set_appendnewvalues/) | Legt einen Wert fest, der angibt, ob neue zu einem Projekt hinzugefügte Werte automatisch zur Liste hinzugefügt werden. |
| [set_AutoRollDown](./set_autorolldown/) | Legt einen Wert fest, der angibt, ob ein automatisches Roll‑Down zu Zuweisungen aktiviert ist. |
| [set_CalculationType](./set_calculationtype/) | Legt den Berechnungstyp des Werts des benutzerdefinierten Attributs fest. |
| [set_Default](./set_default/) | Legt den Standardwert in der Liste fest. |
| [set_DefaultGuid](./set_defaultguid/) | Legt die GUID des Standard‑Lookup‑Tabelleneintrags fest. |
| [set_ElementType](./set_elementtype/) | Legt fest, dass das erweiterte Attribut mit einer Aufgabe, einer Ressource oder einer Zuweisung verknüpft ist. |
| [set_FieldId](./set_fieldid/) | Legt die Projekt‑ID eines benutzerdefinierten Feldes fest. Verwenden Sie die Zeichenkettenrepräsentation einer Konstante aus der Klasse Aspose::Tasks::ExtendedAttributeTask, um die Eigenschaft FieldId anzugeben. |
| [set_Formula](./set_formula/) | Legt die Formel fest, die Microsoft Project verwendet, um ein benutzerdefiniertes Aufgabefeld zu füllen. |
| [set_GraphicalIndicator](./set_graphicalindicator/) | Legt die mit dem erweiterten Attribut verknüpften grafischen Indikatorinformationen fest. Anwendbar auf das MPP‑Format. |
| [set_Guid](./set_guid/) | Legt die GUID eines benutzerdefinierten Feldes fest. |
| [set_MaxMultiValues](./set_maxmultivalues/) | Legt die maximale Anzahl von Werten fest, die Sie in einer Auswahlliste festlegen können. |
| [set_PhoneticsAlias](./set_phoneticsalias/) | Legt die phonetische Aussprache des Alias eines benutzerdefinierten Feldes fest. |
| [set_RestrictValues](./set_restrictvalues/) | Legt einen Wert fest, der angibt, ob die Werte des benutzerdefinierten Feldes auf Werte in der ValueList beschränkt sind. |
| [set_RollupType](./set_rolluptype/) | Legt fest, wie Roll‑Ups berechnet werden. |
| [set_SecondaryGuid](./set_secondaryguid/) | Legt die sekundäre GUID des erweiterten Attributs fest. |
| [set_SecondaryPid](./set_secondarypid/) | Legt die sekundäre PID eines benutzerdefinierten Feldes fest. |
| [set_SummaryRowsCalculationType](./set_summaryrowscalculationtype/) | Legt den Berechnungstyp des Werts des benutzerdefinierten Attributs für Zusammenfassungszeilen fest. |
| [set_UserDef](./set_userdef/) | Legt einen Wert fest, der angibt, ob ein benutzerdefiniertes Feld vom Benutzer definiert ist. |
| [set_ValuelistSortOrder](./set_valuelistsortorder/) | Legt fest, wie Wertlisten sortiert werden. Werte sind: 0=Absteigend, 1=Aufsteigend. |

