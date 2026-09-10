---
title: "CalendarException"
second_title: "Referencia de API de Aspose.Tasks para Python vía .NET"
description: 
type: docs
weight: 160
url: /es/python-net/aspose.tasks/calendarexception/
---

## CalendarException class

Representa períodos de tiempo excepcionales en un calendario.

El tipo CalendarException expone los siguientes miembros:
## Constructores
| Nombre | Descripción |
| :- | :- |
| CalendarException() | Inicializa una nueva instancia de la clase [CalendarException](/tasks/python-net/aspose.tasks/calendarexception/). |
## Propiedades
| Nombre | Descripción |
| :- | :- |
| entered_by_occurrences | Obtiene o establece un valor que indica si el rango de recurrencia se define ingresando un número de ocurrencias.<br/>            False especifica que el rango de recurrencia se define ingresando una fecha de finalización. |
| from_date | Obtiene o establece el inicio del tiempo de la excepción. |
| to_date | Obtiene o establece el final del tiempo de la excepción. |
| occurrences | Obtiene o establece el número de ocurrencias para las que la excepción del calendario es válida. |
| name | Obtiene o establece el nombre de la excepción. |
| type | Obtiene o establece el tipo de excepción. |
| period | Obtiene o establece el período de recurrencia de la excepción. |
| days_of_week | Obtiene la DayTypeCollection para este objeto.<br/>            Los días de la semana en los que la excepción es válida. |
| month_item | Obtiene o establece el elemento de mes para el cual se programa una recurrencia de excepción. |
| month_position | Obtiene o establece la posición de un elemento de mes dentro de un mes. |
| mes | Obtiene o establece el mes para el cual se programa una recurrencia de excepción. |
| month_day | Obtiene o establece el día del mes en el que se programa una recurrencia de excepción. |
| day_working | Obtiene o establece un valor que indica si la fecha o el tipo de día especificado es laborable. |
| working_times | Obtiene o establece el objeto WorkingTimeCollection.<br/>            La colección de tiempos de trabajo que define el tiempo trabajado en el día laborable. |
| parent_calendar | Obtiene el calendario principal para este objeto. |
## Métodos
| Nombre | Descripción |
| :- | :- |
| delete() | Elimina la instancia Exception del objeto CalendarExceptionCollection del calendario padre. |
| check_exception(dt) | Devuelve true si la instancia especificada de la estructura datetime es el día de excepción. |
| get_working_time() | Devuelve el tiempo de trabajo para una excepción de calendario. |
| get_exception_dates() | Devuelve las fechas en las que la excepción de calendario es aplicable. |

### Ver también

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

