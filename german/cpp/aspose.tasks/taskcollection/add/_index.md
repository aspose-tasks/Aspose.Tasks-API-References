---
title: "Aspose::Tasks::TaskCollection::Add Methode"
linktitle: "Add"
articleTitle: "Add"
second_title: "Aspose.Tasks für C++"
description: "Fügt eine neue Aufgabe zur Aufgabensammlung des Projekts auf derselben Gliederungsebene wie die letzte Aufgabe hinzu."
type: docs
weight: 10
url: /de/cpp/aspose.tasks/taskcollection/add/
---

## Add (1 of 5) {#add_1}

Fügt eine neue Aufgabe zur Aufgabensammlung des Projekts auf derselben Gliederungsebene wie die letzte Aufgabe hinzu.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add()
```

---

## Add (2 of 5) {#add_2}

Fügt eine neue Aufgabe vor einer Aufgabe mit der angegebenen ID und auf derselben Gliederungsebene ein.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add(const System::SharedPtr< RecurringTaskParameters > & parameters)
```

| Parameter | Beschreibung |
| --- | --- |
| Parameter | Die Parameter die angegebenen Parameter für die Erstellung einer wiederkehrenden Aufgabe. |

---

## Add (3 of 5) {#add_3}

Fügen Sie die angegebene Aufgabe zur Instanz der Klasse TaskCollection hinzu. Wenn ParentProject.CalculationMode None ist, sollte der Benutzer nach der Verwendung dieser Methode Project.Recalculate() aufrufen (Sie wird alle Projektaufgaben neu planen (Start-/Enddaten, legt frühe/späte Daten fest) und die abhängigen Felder wie Puffer, Arbeits- und Kostendaten, IDs und Gliederungsebenen berechnen). Wenn ParentProject.CalculationMode Manual ist, berechnet die Methode nur die Aufgaben-ID, die Gliederungsebene und die Gliederungsnummern automatisch. Wenn ParentProject.CalculationMode Automatic ist, plant die Methode alle Projektaufgaben automatisch neu (Start-/Enddaten, legt frühe/späte Daten fest, berechnet Puffer, Arbeits- und Kostendaten, berechnet IDs und Gliederungsebenen neu).

**Returns:** void Aspose::Tasks::

```cpp
Add(const System::SharedPtr< Task > & item)
```

| Parameter | Beschreibung |
| --- | --- |
| Element | die angegebene Aufgabe, die zu dieser Aufgabensammlung hinzugefügt werden soll. |

---

## Add (4 of 5) {#add_4}

Fügt eine neue Aufgabe zur Sammlung von Unteraufgaben hinzu.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add(const System::String & taskName)
```

| Parameter | Beschreibung |
| --- | --- |
| taskName | der angegebene Aufgabenname. |

---

## Add (5 of 5) {#add_5}

Fügt eine neue wiederkehrende Aufgabe zur Sammlung von Unteraufgaben hinzu.

**Returns:** returns a task which was inserted before a task with the specified id.

```cpp
Add(const System::String & taskName, int32_t beforeTaskId)
```

| Parameter | Beschreibung |
| --- | --- |
| taskName | der angegebene Aufgabenname. |
| beforeTaskId | Die angegebene ID einer Aufgabe, vor der eine neue Aufgabe eingefügt wird. |

