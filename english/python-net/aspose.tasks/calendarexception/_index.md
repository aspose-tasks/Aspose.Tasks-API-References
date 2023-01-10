---
title: CalendarException
second_title: Aspose.Sildes for Python via .NET API Reference
description: 
type: docs
weight: 170
url: /python-net/aspose.tasks/calendarexception/
---

## CalendarException class

Represent exceptional time periods in a calendar.

The CalendarException type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|CalendarException()|Initializes a new instance of the|
## Properties
| Name | Description |
| :- | :- |
|entered_by_occurrences|Gets or sets a value indicating whether the range of recurrence is defined by entering a number of occurrences.<br/>            False specifies that the range of recurrence is defined by entering a finish date.|
|from_date|Gets or sets the beginning of the exception time.|
|to_date|Gets or sets the end of the exception time.|
|occurrences|Gets or sets the number of occurrences for which the calendar exception is valid.|
|name|Gets or sets the name of the exception.|
|type|Gets or sets the exception type.|
|period|Gets or sets the period of recurrence for the exception.|
|days_of_week|Gets the DayTypeCollection for this object.<br/>            The days of the week on which the exception is valid.|
|month_item|Gets or sets the month item for which an exception recurrence is scheduled.|
|month_position|Gets or sets the position of a month item within a month.|
|month|Gets or sets the month for which an exception recurrence is scheduled.|
|month_day|Gets or sets the day of a month on which an exception recurrence is scheduled.|
|day_working|Gets or sets a value indicating whether the specified date or day type is working.|
|working_times|Gets or sets the WorkingTimeCollection object.<br/>            The collection of working times that defines the time worked on the weekday.|
|parent_calendar|Gets the parent calendar for this object.|
## Methods
| Name | Description |
| :- | :- |
|delete()|Deletes the Exception instance from parent calendar CalendarExceptionCollection object.|
|check_exception(dt)|Returns true if the specified instance of the|
|get_working_time()|Returns the working time for a calendar exception.|
|get_exception_dates()|Returns dates on which the calendar exception is applicable.|

### See Also

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

