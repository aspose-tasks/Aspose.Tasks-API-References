---
title: ExtendedAttributeDefinition
second_title: Aspose.Tasks für .NET-API-Referenz
description: Stellt eine erweiterte Attributdefinition dar die einem Projekt zugeordnet ist.
type: docs
weight: 530
url: /de/net/aspose.tasks/extendedattributedefinition/
---
## ExtendedAttributeDefinition class

Stellt eine erweiterte Attributdefinition dar, die einem Projekt zugeordnet ist.

```csharp
public class ExtendedAttributeDefinition
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Alias](../../aspose.tasks/extendedattributedefinition/alias) { get; set; } | Ruft den Alias eines benutzerdefinierten Felds ab oder legt ihn fest. |
| [AppendNewValues](../../aspose.tasks/extendedattributedefinition/appendnewvalues) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob neu zu einem Projekt hinzugefügte Werte automatisch zur Liste hinzugefügt werden. |
| [AutoRollDown](../../aspose.tasks/extendedattributedefinition/autorolldown) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob ein automatischer Rolldown zu Zuweisungen aktiviert ist. |
| [CalculationType](../../aspose.tasks/extendedattributedefinition/calculationtype) { get; set; } | Ruft die Art der Berechnung des Werts des benutzerdefinierten Attributs ab oder legt sie fest. |
| [CfType](../../aspose.tasks/extendedattributedefinition/cftype) { get; } | Ruft den Typ eines benutzerdefinierten Felds ab. |
| [Default](../../aspose.tasks/extendedattributedefinition/default) { get; set; } | Ruft den Standardwert in der Liste ab oder legt ihn fest. |
| [DefaultGuid](../../aspose.tasks/extendedattributedefinition/defaultguid) { get; set; } | Ruft die Guid des Standard-Nachschlagetabelleneintrags ab oder legt sie fest. |
| [ElementType](../../aspose.tasks/extendedattributedefinition/elementtype) { get; set; } | Ruft ab oder setzt das erweiterte Attribut ist zugeordnet mit einer Aufgabe, einer Ressource oder einer Zuordnung. |
| [FieldId](../../aspose.tasks/extendedattributedefinition/fieldid) { get; set; } | Erhält oder setzt die Projekt-ID eines benutzerdefinierten Felds. Verwenden Sie die Zeichenfolgendarstellung einer Konstante von[`ExtendedAttributeTask`](../extendedattributetask) Klasse zu spezifizieren[`FieldId`](./fieldid) Eigentum. |
| [FieldName](../../aspose.tasks/extendedattributedefinition/fieldname) { get; } | Ruft den Namen eines benutzerdefinierten Felds ab. |
| [Formula](../../aspose.tasks/extendedattributedefinition/formula) { get; set; } | Ruft die Formel ab oder legt sie fest, die Microsoft Project verwendet, um ein benutzerdefiniertes Aufgabenfeld auszufüllen. |
| [Guid](../../aspose.tasks/extendedattributedefinition/guid) { get; set; } | Ruft die Guid eines benutzerdefinierten Felds ab oder legt sie fest. |
| [LookupUid](../../aspose.tasks/extendedattributedefinition/lookupuid) { get; } | Ruft eine Guid der Nachschlagetabelle ab, die einem benutzerdefinierten Feld zugeordnet ist. |
| [MaxMultiValues](../../aspose.tasks/extendedattributedefinition/maxmultivalues) { get; set; } | Ruft die maximale Anzahl von Werten ab oder legt sie fest, die Sie in einer Auswahlliste festlegen können. |
| [ParentProject](../../aspose.tasks/extendedattributedefinition/parentproject) { get; } | Ruft das übergeordnete Projekt für die ab[`ExtendedAttributeDefinition`](../extendedattributedefinition) Instanz. |
| [PhoneticsAlias](../../aspose.tasks/extendedattributedefinition/phoneticsalias) { get; set; } | Ruft die phonetische Aussprache des Alias eines benutzerdefinierten Felds ab oder legt sie fest. |
| [RestrictValues](../../aspose.tasks/extendedattributedefinition/restrictvalues) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob die benutzerdefinierten Feldwerte auf Werte in beschränkt sind[`ValueList`](./valuelist) . |
| [RollupType](../../aspose.tasks/extendedattributedefinition/rolluptype) { get; set; } | Ruft ab oder legt fest, wie Rollups berechnet werden. |
| [SecondaryGuid](../../aspose.tasks/extendedattributedefinition/secondaryguid) { get; set; } | Ruft die sekundäre GUI des erweiterten Attributs ab oder legt sie fest. |
| [SecondaryPid](../../aspose.tasks/extendedattributedefinition/secondarypid) { get; set; } | Ruft die sekundäre PID eines benutzerdefinierten Felds ab oder legt sie fest. |
| [SummaryRowsCalculationType](../../aspose.tasks/extendedattributedefinition/summaryrowscalculationtype) { get; set; } | Ruft den Berechnungstyp des Werts des benutzerdefinierten Attributs für Zusammenfassungszeilen ab oder legt ihn fest. |
| [UserDef](../../aspose.tasks/extendedattributedefinition/userdef) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob ein benutzerdefiniertes Feld benutzerdefiniert ist. |
| [ValueList](../../aspose.tasks/extendedattributedefinition/valuelist) { get; } | Ruft die Liste&lt;Wert&gt; ValueList ab. |
| [ValuelistSortOrder](../../aspose.tasks/extendedattributedefinition/valuelistsortorder) { get; set; } | Ermittelt oder legt fest, wie Wertelisten sortiert werden. Werte sind: 0=Absteigend, 1=Aufsteigend. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition#createlookupresourcedefinition_1)(ExtendedAttributeResource, string) | Factory-Methode, die eine erweiterte Attributdefinition mit Lookup erstellt. Es hat[`CalculationType`](./calculationtype) ist gleichLookup und kann nur in Ressourcen verwendet werden. Sie müssen angeben*fieldId* und*alias* beim Aufruf dieser Methode. Der Feldtyp wird aus der Feld-ID abgeleitet. |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition#createlookupresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Factory-Methode, die eine erweiterte Attributdefinition mit Lookup erstellt. Es hat[`CalculationType`](./calculationtype) ist gleichLookup und kann nur in Ressourcen verwendet werden. Sie müssen angeben*customFieldType* ,*fieldId* und*alias* beim Aufruf dieser Methode. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition#createlookuptaskdefinition_1)(ExtendedAttributeTask, string) | Factory-Methode, die eine erweiterte Attributdefinition mit Lookup erstellt. Es hat[`CalculationType`](./calculationtype) ist gleichLookup und kann nur in Aufgaben verwendet werden. Sie müssen angeben*fieldId* und*alias* beim Aufruf dieser Methode. Der Feldtyp wird aus der Feld-ID abgeleitet. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition#createlookuptaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Factory-Methode, die eine erweiterte Attributdefinition mit Lookup erstellt. Es hat[`CalculationType`](./calculationtype) ist gleichLookup und kann nur in Aufgaben verwendet werden. Sie müssen angeben*customFieldType* ,*fieldId* und*alias* beim Aufruf dieser Methode. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition#createresourcedefinition_1)(ExtendedAttributeResource, string) | Factory-Methode, die eine einfache erweiterte Attributdefinition erstellt, die Microsoft Project als "None" anzeigt. Hat sie[`CalculationType`](./calculationtype) ist gleichNone und kann nur in Ressource verwendet werden. Sie müssen angeben*fieldId* und*alias* beim Aufruf dieser Methode. Der Feldtyp wird aus der Feld-ID abgeleitet. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition#createresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Factory-Methode, die eine einfache erweiterte Attributdefinition erstellt, die Microsoft Project als "None" anzeigt. Hat sie[`CalculationType`](./calculationtype) ist gleichNone und kann nur in Ressource verwendet werden. Sie müssen angeben*customFieldType* ,*fieldId* und*alias* beim Aufruf dieser Methode. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition#createtaskdefinition_1)(ExtendedAttributeTask, string) | Factory-Methode, die eine einfache erweiterte Attributdefinition erstellt, die Microsoft Project als "None" anzeigt. Hat sie[`CalculationType`](./calculationtype) ist gleichNone und kann nur in Aufgaben verwendet werden. Sie müssen angeben*fieldId* und*alias* beim Aufruf dieser Methode. Der Feldtyp wird aus der Feld-ID abgeleitet. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition#createtaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Factory-Methode, die eine einfache erweiterte Attributdefinition erstellt, die Microsoft Project als "None" anzeigt. Hat sie[`CalculationType`](./calculationtype) ist gleichNone und kann nur in Aufgaben verwendet werden. Sie müssen angeben*customFieldType* ,*fieldId* und*alias* beim Aufruf dieser Methode. |
| [AddLookupValue](../../aspose.tasks/extendedattributedefinition/addlookupvalue)(Value) | Fügt der internen Nachschlageliste einen Wert hinzu. Dies ist ein bevorzugter Weg für Manipulationen mit dem[`ValueList`](./valuelist) . |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute)() | Erstellt ein neues erweitertes Attribut mit der Feld-ID, die dem Feld-ID-Wert dieses Objekts entspricht. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_3)(bool) | Erstellt ein neues erweitertes Attribut mit der Feld-ID, die dem Feld-ID-Wert dieses Objekts und dem angegebenen Flag-Wert entspricht. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_4)(DateTime) | Erstellt ein neues erweitertes Attribut mit der Feld-ID, die dem Feld-ID-Wert dieses Objekts und dem angegebenen Datumswert entspricht. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_5)(decimal) | Erstellt ein neues erweitertes Attribut mit der Feld-ID, die dem Feld-ID-Wert dieses Objekts und dem angegebenen numerischen Wert entspricht. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_1)(Duration) | Erstellt ein neues erweitertes Attribut mit der Feld-ID, die dem Feld-ID-Wert dieses Objekts und dem angegebenen Dauerwert entspricht. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_6)(string) | Erstellt ein neues erweitertes Attribut mit der Feld-ID, die dem Feld-ID-Wert dieses Objekts und dem angegebenen Textwert entspricht. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_2)(Value) | Erstellt ein neues erweitertes Attribut, das mit dem angegebenen verknüpft ist[`Value`](../value) Artikel. |
| override [Equals](../../aspose.tasks/extendedattributedefinition/equals)(object) | Gibt ein Flag zurück, das angibt, ob diese Instanz gleich dem angegebenen Objekt ist. |
| override [GetHashCode](../../aspose.tasks/extendedattributedefinition/gethashcode)() | Gibt einen Hashcode für die Instanz von zurück[`ExtendedAttributeDefinition`](../extendedattributedefinition) Klasse. |
| [RemoveLookupValue](../../aspose.tasks/extendedattributedefinition/removelookupvalue)(Value) | Entfernt einen Wert aus der internen Nachschlageliste. Dies ist ein bevorzugter Weg für Manipulationen mit dem[`ValueList`](./valuelist) . |

### Siehe auch

* namensraum [Aspose.Tasks](../../aspose.tasks)
* Montage [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
