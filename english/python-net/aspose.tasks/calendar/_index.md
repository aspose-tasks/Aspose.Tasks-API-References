---
title: Calendar
second_title: Aspose.Tasks for Python via .NET API Reference
description: 
type: docs
weight: 140
url: /python-net/aspose.tasks/calendar/
---

## Calendar class

Represents a calendar used in a project.

The Calendar type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|name|Gets or sets the name of the calendar.|
|uid|Gets or sets the unique identifier of the calendar.|
|week_days|Gets WeekDaysCollection for this calendar.<br/>            The collection of weekdays that defines the calendar.|
|exceptions|Gets CalendarExceptionCollection object.<br/>            The collection of exceptions that is associated with the calendar.|
|work_weeks|Gets WorkWeekCollections object.<br/>            The collection of work weeks that is associated with the calendar.|
|is_base_calendar|Gets a value indicating whether the calendar is a base calendar.|
|base_calendar|Gets or sets the base calendar on which this calendar depends.<br/>            Only applicable if the calendar is not a base calendar.|
|is_baseline_calendar|Gets or sets a value indicating whether the calendar is a baseline calendar.|
|guid|Gets calendar's Guid.|
## Methods
| Name | Description |
| :- | :- |
|get_start_date_from_finish_and_duration(finish, duration)|Returns StartDate based on specified FinishDate and Duration.|
|get_start_date_from_finish_and_duration(finish, duration)|Returns StartDate based on specified FinishDate and Duration.|
|get_working_hours(start, finish)|Return working hours for the specified dates.|
|get_working_hours(dt)|Return working hours for the specified dates.|
|get_finish_date_by_start_and_work(start, work)|Calculates the date when the specified amount of work time will pass according to the calendar.|
|get_finish_date_by_start_and_work(start, work)|Calculates the date when the specified amount of work time will pass according to the calendar.|
|make_standard_calendar(calendar)|Creates default standard calendar.|
|make_24_hour_calendar(calendar)|Makes a given Calendar to be a 24Hour Calendar.<br/>            24Hours Calendar is a Calendar in which every day of week is working with Round-the-clock working hours.|
|make_night_shift_calendar(calendar)|Makes a given Calendar as Night Shift Calendar.|
|delete()|Removes calendar from project.|
|is_day_working(dt)|Determines whether the day is working day.|
|get_task_finish_date_from_duration(task, duration)|Calculates the task finish date and time from its start date, split parts and the duration.|
|get_working_times(dt)|Returns [WorkingTimeCollection](/tasks/python-net/aspose.tasks/workingtimecollection/) of working times for the specified date.|
|get_previous_working_day_end(date)|Calculates previous working date end from the specified date.|
|get_next_working_day_start(date)|Calculates next working day start from the date.|

### See Also

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

