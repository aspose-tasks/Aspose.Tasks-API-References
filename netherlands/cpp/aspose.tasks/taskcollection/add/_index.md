---
title: "Aspose::Tasks::TaskCollection::Add methode"
linktitle: "Toevoegen"
articleTitle: "Toevoegen"
second_title: "Aspose.Tasks voor C++"
description: "Voegt een nieuwe taak toe aan de projecttaken-collectie op hetzelfde outline-niveau als de laatste taak."
type: docs
weight: 10
url: /nl/cpp/aspose.tasks/taskcollection/add/
---

## Add (1 of 5) {#add_1}

Voegt een nieuwe taak toe aan de projecttaken-collectie op hetzelfde outline-niveau als de laatste taak.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add()
```

---

## Add (2 of 5) {#add_2}

Voegt een nieuwe taak in vóór een taak met de opgegeven id en op hetzelfde outline‑niveau.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add(const System::SharedPtr< RecurringTaskParameters > & parameters)
```

| Parameter | Beschrijving |
| --- | --- |
| parameters | De parameters die zijn opgegeven voor het maken van een terugkerende taak. |

---

## Add (3 of 5) {#add_3}

Voeg de opgegeven taak toe aan de instantie van de TaskCollection‑klasse. Als ParentProject.CalculationMode None is, moet de gebruiker Project.Recalculate() aanroepen na het gebruik van deze methode (Dit zal alle projecttaken herschikken (start-/einddatums, stelt vroege/late datums in) en de afhankelijke velden berekenen, zoals slack, werk‑ en kostengegevens, id’s en outline‑niveaus). Als ParentProject.CalculationMode Manual is, berekent de methode alleen taak‑id, outline‑niveau en outline‑nummers automatisch. Als ParentProject.CalculationMode Automatic is, herschikt de methode alle taken van het project automatisch (start-/einddatums, stelt vroege/late datums in, berekent slack, werk‑ en kostengegevens, herberekent id’s en outline‑niveaus).

**Returns:** void Aspose::Tasks::

```cpp
Add(const System::SharedPtr< Task > & item)
```

| Parameter | Beschrijving |
| --- | --- |
| item | de opgegeven taak die aan deze taakverzameling moet worden toegevoegd. |

---

## Add (4 of 5) {#add_4}

Voegt een nieuwe taak toe aan de verzameling van onderliggende taken.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add(const System::String & taskName)
```

| Parameter | Beschrijving |
| --- | --- |
| taskName | de opgegeven taaknaam. |

---

## Add (5 of 5) {#add_5}

Voegt een nieuwe terugkerende taak toe aan de verzameling van onderliggende taken.

**Returns:** returns a task which was inserted before a task with the specified id.

```cpp
Add(const System::String & taskName, int32_t beforeTaskId)
```

| Parameter | Beschrijving |
| --- | --- |
| taskName | de opgegeven taaknaam. |
| beforeTaskId | De opgegeven id van een taak vóór welke een nieuwe taak wordt ingevoegd. |

