---
title: "CalendarException"
second_title: "Aspose.Tasks pour Python via .NET Référence de l'API"
description: 
type: docs
weight: 160
url: /fr/python-net/aspose.tasks/calendarexception/
---

## CalendarException class

Représente des périodes de temps exceptionnelles dans un calendrier.

Le type CalendarException expose les membres suivants :
## Constructeurs
| Nom | Description |
| :- | :- |
| CalendarException() | Initialise une nouvelle instance de la classe [CalendarException](/tasks/python-net/aspose.tasks/calendarexception/). |
## Propriétés
| Nom | Description |
| :- | :- |
| entered_by_occurrences | Obtient ou définit une valeur indiquant si la plage de récurrence est définie en saisissant un nombre d'occurrences.<br/>            False indique que la plage de récurrence est définie en saisissant une date de fin. |
| from_date | Obtient ou définit le début de l'heure de l'exception. |
| to_date | Obtient ou définit la fin de l'heure de l'exception. |
| occurrences | Obtient ou définit le nombre d'occurrences pour lesquelles l'exception de calendrier est valide. |
| name | Obtient ou définit le nom de l'exception. |
| type | Obtient ou définit le type d'exception. |
| period | Obtient ou définit la période de récurrence de l'exception. |
| days_of_week | Obtient le DayTypeCollection pour cet objet.<br/>            Les jours de la semaine pendant lesquels l'exception est valide. |
| month_item | Obtient ou définit l'élément de mois pour lequel une récurrence d'exception est planifiée. |
| month_position | Obtient ou définit la position d'un élément de mois au sein d'un mois. |
| mois | Obtient ou définit le mois pour lequel une récurrence d'exception est planifiée. |
| month_day | Obtient ou définit le jour du mois auquel une récurrence d'exception est planifiée. |
| day_working | Obtient ou définit une valeur indiquant si la date ou le type de jour spécifié est travaillé. |
| working_times | Obtient ou définit l'objet WorkingTimeCollection.<br/>            La collection des horaires de travail qui définit le temps travaillé pendant la semaine. |
| parent_calendar | Obtient le calendrier parent de cet objet. |
## Méthodes
| Nom | Description |
| :- | :- |
| delete() | Supprime l'instance Exception du calendrier parent CalendarExceptionCollection. |
| check_exception(dt) | Renvoie true si l'instance spécifiée de la structure datetime correspond au jour d'exception. |
| get_working_time() | Renvoie le temps de travail pour une exception de calendrier. |
| get_exception_dates() | Renvoie les dates auxquelles l'exception de calendrier s'applique. |

### Voir aussi

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

