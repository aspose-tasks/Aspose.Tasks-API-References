---
title: "Calendar"
second_title: "Referencia de API de Aspose.Tasks para Python vía .NET"
description: 
type: docs
weight: 140
url: /es/python-net/aspose.tasks/calendar/
---

## Calendar class

Representa un calendario usado en un proyecto.

El tipo Calendar expone los siguientes miembros:
## Propiedades
| Nombre | Descripción |
| :- | :- |
| name | Obtiene o establece el nombre del calendario. |
| uid | Obtiene o establece el identificador único del calendario. |
| week_days | Obtiene WeekDaysCollection para este calendario.<br/>            La colección de días de la semana que define el calendario. |
| exceptions | Obtiene el objeto CalendarExceptionCollection.<br/>            La colección de excepciones asociada al calendario. |
| work_weeks | Obtiene el objeto WorkWeekCollections.<br/>            La colección de semanas laborables asociada al calendario. |
| is_base_calendar | Obtiene un valor que indica si el calendario es un calendario base. |
| base_calendar | Obtiene o establece el calendario base del cual depende este calendario.<br/>            Sólo aplicable si el calendario no es un calendario base. |
| is_baseline_calendar | Obtiene o establece un valor que indica si el calendario es un calendario de línea base. |
| guid | Obtiene el Guid del calendario. |
| primavera_properties | Obtiene un objeto que contiene propiedades específicas de Primavera para un calendario leído de formatos Primavera. |
## Métodos
| Nombre | Descripción |
| :- | :- |
| get_start_date_from_finish_and_duration(finish, duration) | Devuelve la fecha de inicio basada en la fecha de fin y duración especificadas. |
| get_start_date_from_finish_and_duration(finish, duration) | Devuelve la fecha de inicio basada en la fecha de fin y duración especificadas. |
| get_working_hours(start, finish) | Devuelve WorkUnit - Inicio, Fin y Duración de las horas laborables para el intervalo de fecha y hora especificado. |
| get_working_hours(dt) | Devuelve WorkUnit - Inicio, Fin y Duración de las horas laborables para el intervalo de fecha y hora especificado. |
| get_finish_date_by_start_and_work(start, work) | Calcula la fecha en que el tiempo de trabajo especificado transcurrirá según el calendario. |
| get_finish_date_by_start_and_work(start, work) | Calcula la fecha en que el tiempo de trabajo especificado transcurrirá según el calendario. |
| get_intersection_calendar(calendar1, calendar2) | Obtiene la instancia [ICalendar](/tasks/python-net/aspose.tasks/icalendar/) que puede usarse para realizar cálculos sobre la intersección de los horarios de trabajo de 2 calendarios. |
| make_standard_calendar(calendar) | Crea un calendario estándar predeterminado. |
| make_24_hour_calendar(calendar) | Convierte un Calendario dado en un Calendario de 24 Horas.<br/>            El Calendario de 24 Horas es un Calendario en el que cada día de la semana trabaja con horario continuo las 24 horas. |
| make_night_shift_calendar(calendar) | Convierte un Calendario dado en un Calendario de Turno Nocturno. |
| delete() | Elimina el calendario del proyecto. |
| is_day_working(dt) | Determina si el día especificado es un día laborable según el calendario. |
| get_working_hours_time_span(start, finish) | Devuelve la cantidad de horas laborables entre las fechas especificadas. |
| get_task_finish_date_from_duration(task, duration) | Calcula la fecha y hora de finalización de la tarea a partir de su fecha de inicio, partes divididas y la duración del trabajo. |
| get_working_times(dt) | Devuelve una [WorkingTimeCollection](/tasks/python-net/aspose.tasks/workingtimecollection/) de tiempos de trabajo para la fecha especificada. |
| get_previous_working_day_end(date) | Calcula el final del día laborable anterior a partir de la fecha especificada. |
| get_next_working_day_start(date) | Calcula el inicio del siguiente día laborable para la fecha especificada. |
| get_work_start(date) | Calcula el inicio del siguiente tiempo laborable a partir de la fecha y hora especificadas. |
| is_empty() | Devuelve si el calendario no tiene horas laborables definidas. |

### Ver también

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

