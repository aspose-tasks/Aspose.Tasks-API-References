---
title: "Calendar"
second_title: "Aspose.Tasks pour Python via .NET Référence de l'API"
description: 
type: docs
weight: 140
url: /fr/python-net/aspose.tasks/calendar/
---

## Calendar class

Représente un calendrier utilisé dans un projet.

Le type Calendar expose les membres suivants:
## Propriétés
| Nom | Description |
| :- | :- |
| name | Obtient ou définit le nom du calendrier. |
| uid | Obtient ou définit l'identifiant unique du calendrier. |
| week_days | Obtient WeekDaysCollection pour ce calendrier.<br/>            La collection des jours de la semaine qui définit le calendrier. |
| exceptions | Obtient l'objet CalendarExceptionCollection.<br/>            La collection des exceptions associée au calendrier. |
| work_weeks | Obtient l'objet WorkWeekCollections.<br/>            La collection des semaines de travail associée au calendrier. |
| is_base_calendar | Obtient une valeur indiquant si le calendrier est un calendrier de base. |
| base_calendar | Obtient ou définit le calendrier de base dont dépend ce calendrier.<br/>            Applicable uniquement si le calendrier n'est pas un calendrier de base. |
| is_baseline_calendar | Obtient ou définit une valeur indiquant si le calendrier est un calendrier de référence. |
| guid | Obtient le Guid du calendrier. |
| primavera_properties | Obtient un objet contenant les propriétés spécifiques à Primavera pour un calendrier lu à partir des formats Primavera. |
## Méthodes
| Nom | Description |
| :- | :- |
| get_start_date_from_finish_and_duration(finish, duration) | Renvoie la date de début basée sur la date de fin et la durée spécifiées. |
| get_start_date_from_finish_and_duration(finish, duration) | Renvoie la date de début basée sur la date de fin et la durée spécifiées. |
| get_working_hours(start, finish) | Renvoie WorkUnit - Début, Fin et Durée des heures de travail pour l'intervalle de temps spécifié. |
| get_working_hours(dt) | Renvoie WorkUnit - Début, Fin et Durée des heures de travail pour l'intervalle de temps spécifié. |
| get_finish_date_by_start_and_work(start, work) | Calcule la date à laquelle la quantité spécifiée de temps de travail sera écoulée selon le calendrier. |
| get_finish_date_by_start_and_work(start, work) | Calcule la date à laquelle la quantité spécifiée de temps de travail sera écoulée selon le calendrier. |
| get_intersection_calendar(calendar1, calendar2) | Obtient l'instance [ICalendar](/tasks/python-net/aspose.tasks/icalendar/) qui peut être utilisée pour effectuer des calculs sur l'intersection des horaires de travail de 2 calendriers. |
| make_standard_calendar(calendar) | Crée le calendrier standard par défaut. |
| make_24_hour_calendar(calendar) | Transforme un calendrier donné en 24Hour Calendar.<br/>            24Hours Calendar est un calendrier dans lequel chaque jour de la semaine travaille avec des heures de travail continues. |
| make_night_shift_calendar(calendar) | Transforme un calendrier donné en Night Shift Calendar. |
| delete() | Supprime le calendrier du projet. |
| is_day_working(dt) | Détermine si le jour spécifié est un jour ouvrable selon le calendrier. |
| get_working_hours_time_span(start, finish) | Renvoie la quantité d'heures de travail entre les dates spécifiées. |
| get_task_finish_date_from_duration(task, duration) | Calcule la date et l'heure de fin de la tâche à partir de sa date de début, de ses parties fractionnées et de la durée de travail. |
| get_working_times(dt) | Renvoie le [WorkingTimeCollection](/tasks/python-net/aspose.tasks/workingtimecollection/) des temps de travail pour la date spécifiée. |
| get_previous_working_day_end(date) | Calcule la fin de la journée de travail précédente à partir de la date spécifiée. |
| get_next_working_day_start(date) | Calcule le début du prochain jour ouvrable pour la date spécifiée. |
| get_work_start(date) | Calcule le début du prochain temps de travail à partir de la date et de l'heure spécifiées. |
| is_empty() | Renvoie si le calendrier ne possède pas d'heures de travail définies. |

### Voir aussi

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

