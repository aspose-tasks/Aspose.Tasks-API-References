---
title: "TaskCollection"
second_title: "Aspose.Tasks for Python via .NET API-referentie"
description: 
type: docs
weight: 1140
url: /nl/python-net/aspose.tasks/taskcollection/
---

## TaskCollection class

Stelt een verzameling van [Task](/tasks/python-net/aspose.tasks/task/) objecten voor.

Het type TaskCollection biedt de volgende leden:
## Eigenschappen
| Naam | Beschrijving |
| :- | :- |
| parent_project | Haalt het bovenliggende project op van het TaskCollection-object. |
## Methods
| Naam | Beschrijving |
| :- | :- |
| add() | Voeg de opgegeven taak toe aan de instantie van de [TaskCollection](/tasks/python-net/aspose.tasks/taskcollection/) klasse.<br/>            Als ParentProject.CalculationMode None is, moet de gebruiker Project.Recalculate() aanroepen na het gebruik van deze methode (deze zal alle projecttaken opnieuw plannen (start-/einddatums, stelt vroege/late datums in) en de afhankelijke velden berekenen, zoals speling, werk- en kostengegevens, id's en outline-niveaus).<br/>            Als ParentProject.CalculationMode Manual is, berekent de methode alleen taak-id, outline-niveau en outline-nummers automatisch.<br/>            Als ParentProject.CalculationMode Automatic is, plant de methode alle taken van het project automatisch opnieuw<br/>            (start-/einddatums, stelt vroege/late datums in, berekent speling, werk- en kostengegevens, herberekent  id's en outline-niveaus). |
| add(task_name) | Voegt een nieuwe taak toe aan de collectie van onderliggende taken. |
| add(task_name, before_task_id) |  |
| add(parameters) | Voegt een nieuwe taak in vóór een taak met de opgegeven id en op hetzelfde outline-niveau. |
| to_list() | Converteert het TaskCollection-object naar een lijst van [Task](/tasks/python-net/aspose.tasks/task/) objecten. |
| get_by_uid(uid) | Retourneert een taak met de opgegeven Uid waarvan de voorouder de bovenliggende taak van deze collectie is. |
| get_by_id(id) | Retourneert een taak met de opgegeven Id waarvan de voorouder de bovenliggende taak van deze collectie is. |

### Zie ook

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

