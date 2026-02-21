---
title: ICalendar
second_title: Aspose.Tasks for Python via .NET API Reference
description: 
type: docs
weight: 480
url: /python-net/aspose.tasks/icalendar/
---

## ICalendar class

Represents a calendar abstraction which can be used for various calculations of dates and durations.

The ICalendar type exposes the following members:
## Methods
| Name | Description |
| :- | :- |
|get_start_date_from_finish_and_duration(finish, duration)|Returns start date based on the specified finish date and duration.|
|get_start_date_from_finish_and_duration(finish, duration)|Returns start date based on specified finish date and duration.|
|get_working_hours(start, finish)|Returns WorkUnit - Start, Finish and Duration of working hours for the specified date time interval.|
|get_working_hours(dt)|Returns WorkUnit - Start, Finish and Duration of working hours for the specified date time interval.|
|get_finish_date_by_start_and_work(start, work)|Calculates the date when the specified amount of work time will pass according to the calendar.|
|get_finish_date_by_start_and_work(start, work)|Calculates the date when the specified amount of work time will pass according to the calendar.|
|is_day_working(dt)|Determines whether the specified day is a working day according to the calendar.|
|get_working_hours_time_span(start, finish)|Returns amount of working hours between the specified dates.|
|get_task_finish_date_from_duration(task, duration)|Calculates the task finish date and time from its start date, split parts and the work duration.|
|get_working_times(dt)|Returns [WorkingTimeCollection](/tasks/python-net/aspose.tasks/workingtimecollection/) of working times for the specified date.|
|get_previous_working_day_end(date)|Calculates the end of the previous working date from the specified date.|
|get_next_working_day_start(date)|Calculates next working day start for the specified date.|
|get_work_start(date)|Calculates next working time start beginning from the specified date and time.|
|is_empty()|Returns whether the calendar doesn't have working hours defined.|

### See Also

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

