---
title: "TaskCollection"
second_title: "Aspose.Tasks für Python via .NET API-Referenz"
description: 
type: docs
weight: 1140
url: /de/python-net/aspose.tasks/taskcollection/
---

## TaskCollection class

Stellt eine Sammlung von [Task](/tasks/python-net/aspose.tasks/task/) Objekten dar.

Der Typ TaskCollection stellt die folgenden Mitglieder bereit:
## Eigenschaften
| Name | Beschreibung |
| :- | :- |
| parent_project | Ermittelt das übergeordnete Projekt des TaskCollection-Objekts. |
## Methoden
| Name | Beschreibung |
| :- | :- |
| add() | Fügt die angegebene Aufgabe zur Instanz der Klasse [TaskCollection](/tasks/python-net/aspose.tasks/taskcollection/) hinzu.<br/>            Wenn ParentProject.CalculationMode None ist, sollte der Benutzer nach Verwendung dieser Methode Project.Recalculate() aufrufen (es wird alle Projektaufgaben neu planen (Start-/Enddaten, legt frühere/spätere Daten fest) und die abhängigen Felder wie Puffer, Arbeits- und Kostenfelder, IDs und Gliederungsebenen berechnen).<br/>            Wenn ParentProject.CalculationMode Manual ist, berechnet die Methode nur die Aufgaben-ID, Gliederungsebene und Gliederungsnummern automatisch.<br/>            Wenn ParentProject.CalculationMode Automatic ist, plant die Methode alle Projektaufgaben automatisch neu<br/>            (Start-/Enddaten, legt frühere/spätere Daten fest, berechnet Puffer, Arbeits- und Kostenfelder, berechnet IDs und Gliederungsebenen neu). |
| add(task_name) | Fügt eine neue Aufgabe zur Sammlung von Unteraufgaben hinzu. |
| add(task_name, before_task_id) |  |
| add(parameters) | Fügt eine neue Aufgabe vor einer Aufgabe mit der angegebenen ID und auf derselben Gliederungsebene ein. |
| to_list() | Konvertiert das TaskCollection-Objekt in eine Liste von [Task](/tasks/python-net/aspose.tasks/task/)-Objekten. |
| get_by_uid(uid) | Gibt eine Aufgabe mit der angegebenen UID zurück, deren Vorgänger die übergeordnete Aufgabe dieser Sammlung ist . |
| get_by_id(id) | Gibt eine Aufgabe mit der angegebenen ID zurück, deren Vorgänger die übergeordnete Aufgabe dieser Sammlung ist . |

### Siehe auch

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

