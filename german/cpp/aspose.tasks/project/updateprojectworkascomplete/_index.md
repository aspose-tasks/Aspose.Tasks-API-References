---
title: "Aspose::Tasks::Project::UpdateProjectWorkAsComplete Methode"
linktitle: "UpdateProjectWorkAsComplete"
articleTitle: "UpdateProjectWorkAsComplete"
second_title: "Aspose.Tasks für C++"
description: "Aktualisiert alle Arbeiten als abgeschlossen bis zu einem angegebenen Datum für das gesamte Projekt."
type: docs
weight: 2080
url: /de/cpp/aspose.tasks/project/updateprojectworkascomplete/
---

## UpdateProjectWorkAsComplete (1 of 2) {#updateprojectworkascomplete_1}

Aktualisiert alle Arbeiten als abgeschlossen bis zu einem angegebenen Datum für das gesamte Projekt.

**Returns:** void Aspose::Tasks::

```cpp
UpdateProjectWorkAsComplete(System::DateTime completeThrough, bool setZeroOrHundredPercentCompleteOnly)
```

| Parameter | Beschreibung |
| --- | --- |
| completeThrough | Das Datum, um die Arbeit bis zu diesem Zeitpunkt als abgeschlossen zu aktualisieren. |
| setZeroOrHundredPercentCompleteOnly | Wenn auf true gesetzt, werden nur jene Aufgaben als zu 100 % abgeschlossen aktualisiert, deren Enddatum vor dem angegebenen complete-through‑Datum liegt. Andernfalls wird ein prozentualer Abschlusswert basierend auf geplantem Start- und complete-through‑Datum berechnet. |

---

## UpdateProjectWorkAsComplete (2 of 2) {#updateprojectworkascomplete_2}

Aktualisiert die gesamte Arbeit bis zu einem angegebenen Datum für die angegebene Aufgabenliste als abgeschlossen.

**Returns:** void Aspose::Tasks::

```cpp
UpdateProjectWorkAsComplete(System::DateTime completeThrough, bool setZeroOrHundredPercentCompleteOnly, const System::SharedPtr< System::Collections::Generic::List< System::SharedPtr< Task >>> & taskCollection)
```

| Parameter | Beschreibung |
| --- | --- |
| completeThrough | Das Datum, um die Arbeit bis zu diesem Zeitpunkt als abgeschlossen zu aktualisieren. |
| setZeroOrHundredPercentCompleteOnly | Wenn auf true gesetzt, werden nur jene Aufgaben als zu 100 % abgeschlossen aktualisiert, deren Enddatum vor dem angegebenen complete-through‑Datum liegt. Andernfalls wird ein prozentualer Abschlusswert basierend auf geplantem Start- und complete-through‑Datum berechnet. |
| taskCollection | List< Task > von Aufgaben, für die die Arbeit aktualisiert werden soll. |

