---
title: DateLabel
second_title: Aspose.Sildes for Python via .NET API Reference
description: 
type: docs
weight: 290
url: /tasks/python-net/aspose.tasks.visualization/datelabel/
---

## DateLabel enumeration

Specifies the display format for date and time labels in a timescale.

## Members
| Member name | Description |
| :- | :- |
|NONE|No date is displayed.|
|DAY_DDD|Examples are Mon, Tue.|
|DAY_DDD_DD|Examples are Mon 30, Tue 1|
|DAY_DDD_M_DD|Examples are Mon S 30, Tue O 1|
|DAY_DDD_MM_DD|Examples are Mon 9/30, Tue 10/1|
|DAY_DDD_MM_DD_YY|Examples are Mon 9/30/02, Tue 10/1/02|
|DAY_DDD_MMM_DD|Examples are Mon Sep 30, Tue Oct 1|
|DAY_DDD_MMM_DD_YYY|Examples are Mon Sep 30 '02, Tue Oct 1 '02|
|DAY_DDD_MMMM_DD|Examples are Mon September 30, Tue October 1|
|DAY_DDDD|Examples are Tuesday, Wednesday.|
|DAY_DDI|Examples are Mo, Tu|
|DAY_DDI_DD|Examples are Mo 30, Tu 1|
|DAY_DDI_M_DD|Examples are Mo S 30, Tu O 1|
|DAY_DDI_MM_DD|Examples are Mo 9/30, Tu 10/1|
|DAY_DI|Examples are M, T|
|DAY_DI_DD_SPACE|Examples are M 30, T 1|
|DAY_DI_M_DD|Examples are M S 30, T O 1|
|DAY_DI_MM_DD|Examples are M 9/30, T 10/1|
|DAY_DI_DD_NO_SPACE|Examples are M30, T1|
|DAY_M_DD|Examples are S 30, O 1|
|DAY_MM_DD|Examples are 9/30, 10/1|
|DAY_MM_DD_YY|Examples are 9/30/02, 10/1/02|
|DAY_MMM_DD|Examples are Sep 30, Oct 1|
|DAY_MMM_DD_YYY|Examples are Sep 30 '02, Oct 10 '02|
|DAY_FROM_END_DAY_DD|Examples are Day 2, Day 1, Day -1, Day -2 from the project end.|
|DAY_FROM_END_DD|Examples are 2, 1, -1, -2|
|DAY_FROM_END_DDD|Examples are D2, D1, D-1, D-2|
|DAY_FROM_START_DAY_DD|Examples are Day -2, Day -1, Day 1, Day 2 from the project start.|
|DAY_FROM_START_DD|Examples are -2, -1, 1, 2|
|DAY_FROM_START_DDD|Examples are D-2, D-1, D1, D2|
|DAY_OF_MONTH_DD|Examples are 30, 1|
|DAY_OF_YEAR_DD|Examples are 77, 78|
|DAY_OF_YEAR_DD_YYY|Examples are 77 '10, 78 '10|
|DAY_OF_YEAR_DD_YYYY|Examples are 77 2010, 78 2010|
|DAY_DD_MM_YYYY|Example is 19/07/2016.|
|HALF_YEAR_H|Examples are 1, 2. Requires the time unit to be TimescaleHalfYears.|
|HALF_YEAR_HH|Examples are H1, H2|
|HALF_YEAR_HH_YYY|Examples are H1 '10, H2 '10|
|HALF_YEAR_HHH_HALF|Examples are 1st Half, 2d Half|
|HALF_YEAR_H_HYY|Examples are 1H10, 2H10|
|HALF_YEAR_HLF_H|Examples are Half 1, Half 2|
|HALF_YEAR_HLF_H_YYYY|Examples are Half 1, 2010; Half 2, 2010|
|HALF_YEAR_FROM_END_H|Examples are 2, 1, -1, -2. Half years from the project end date.|
|HALF_YEAR_FROM_END_HALF_H|Examples are Half 2, Half 1, Half -1, Half -2|
|HALF_YEAR_FROM_END_HH|Examples are H2, H1, H-1, H-2|
|HALF_YEAR_FROM_START_H|Examples are -2, -1, 1, 2. Half years from the project start date.|
|HALF_YEAR_FROM_START_HALF_H|Examples are Half -2, Half -1, Half 1, Half 2|
|HALF_YEAR_FROM_START_HH|Examples are H-2, H-1, H1, H2|
|HOUR_DDD_MMM_DD_HH_AM|Examples are Wed Mar 18, 8 AM; Wed Mar 18, 9 AM. Requires the time unit to be TimescaleHours.|
|HOUR_HH|Examples are 8, 9, 10, 11|
|HOUR_HH_MM_AM|Examples are 8:00 AM, 9:00 AM|
|HOUR_HH_AM|Examples are 8AM, 9AM|
|HOUR_MM_DD_HH_AM|Examples are 3/18 8 AM, 3/18 9 AM|
|HOUR_MMM_DD_HH_AM|Examples are Mar 18, 8 AM; Mar 18, 9 AM|
|HOUR_FROM_END_HH|Examples are 3, 2, 1, -1, -2 hours from the project end.|
|HOUR_FROM_END_HHH|Examples are H3, H2, H1, H-1, H-2|
|HOUR_FROM_END_HOUR_HH|Examples are Hour 3, Hour 2, Hour 1, Hour -1, Hour -2|
|HOUR_FROM_START_HH|Examples are -2, -1, 1, 2, 3 hours from the project start.|
|HOUR_FROM_START_HHH|Examples are H-2, H-1, H1, H2, H3|
|HOUR_FROM_START_HOUR_HH|Examples are Hour -2, Hour -1, Hour 1, Hour 2, Hour 3|
|MINUTE_HH_MM_AM|Examples are 8:00 AM, 8:01 AM, 8:02 AM. Requires the time unit to be TimescaleMinutes.|
|MINUTE_MM|Examples are 0, 1, 2, ..., 59 minutes|
|MINUTE_FROM_END_MINUTE_MM|Examples are Minute 181, Minute 180, ..., Minute 1, Minute -1 from the project end.|
|MINUTE_FROM_END_MM|Examples are 181, 180, ..., 1, -1|
|MINUTE_FROM_END_MMM|Examples are M181, M180, ..., M1, M-1|
|MINUTE_FROM_START_MINUTE_MM|Examples are Minute -2, Minute -1, Minute 1, ... Minute 180 from the project start.|
|MINUTE_FROM_START_MM|Examples are -2, -1, 1, ..., 180|
|MINUTE_FROM_START_MMM|Examples are M-2, M-1, M1, ..., M180|
|MONTH_M|Examples are M, A, M, J, J. Requires the time unit to be TimescaleMonths.|
|MONTH_MM|Examples are 11, 12, 1, 2|
|MONTH_MM_YY|Examples are 3/10, 4/10, 5/10|
|MONTH_MM_YYY|Examples are 3 '10, 4 '10, 5 '10|
|MONTH_MMM|Examples are Mar, Apr, May|
|MONTH_MMM_YYY|Examples are Mar '10, Apr '10, May '10|
|MONTH_MMMM|Examples are March, April, May|
|MONTH_MMMM_YYYY|Examples are March 2010, April 2010, May 2010|
|MONTH_FROM_END_MM|Examples are 2, 1, -1, -2 months from the project end.|
|MONTH_FROM_END_MMM|Examples are M2, M1, M-1, M-2|
|MONTH_FROM_END_MONTH_MM|Examples are Month 2, Month 1, Month -1, Month -2|
|MONTH_FROM_START_MM|Examples are -2, -2, 1, 2 months from the project start.|
|MONTH_FROM_START_MMM|Examples are M-2, M-1, M1, M2|
|MONTH_FROM_START_MONTH_MM|Examples are Month -2, Month -1, Month 1, Month 2|
|QUARTER_Q|Examples are 3, 4, 1. Requires the time unit to be TimescaleQuarters.|
|QUARTER_QQ|Examples are Q3, Q4, Q1|
|QUARTER_QQ_YYY|Examples are Q3 '10, Q4 '10, Q1 '11|
|QUARTER_QQQ_QUARTER|Examples are 3rd Quarter, 1st Quarter|
|QUARTER_Q_QYY|Examples are 3Q10, 4Q10, 1Q11|
|QUARTER_QTR_Q|Examples are Qtr3, Qtr4, Qtr1|
|QUARTER_QTR_Q_YYYY|Examples are Qtr3, 2010; Qtr4, 2010; Qtr1, 2011|
|QUARTER_FROM_END_Q|Examples are 5, 4, 3, 2, 1, -1 quarters from the project end.|
|QUARTER_FROM_END_QQ|Examples are Q5, Q4, Q3, Q2, Q1, Q-1|
|QUARTER_FROM_END_QUARTER_Q|Examples are Quarter 5, Quarter 4, Quarter 3, Quarter 2, Quarter 1, Quarter -1|
|QUARTER_FROM_START_Q|Examples are -5, -4, -3, -2, -1, 1 quarters from the project start.|
|QUARTER_FROM_START_QQ|Examples are Q-5, Q-4, Q-3, Q-2, Q-1, Q1|
|QUARTER_FROM_START_QUARTER_Q|Examples are Quarter -5, Quarter -4, Quarter -3, Quarter -2, Quarter -1, Quarter 1|
|THIRDS_OF_MONTHS_DD|Examples are 1, 11, 21, 1. Requires the time unit to be TimescaleThirdsOfMonths.|
|THIRDS_OF_MONTHS_DDD|Examples are B, M, E, B|
|THIRDS_OF_MONTHS_DDDD|Examples are Beginning, Middle, End, Beginning|
|THIRDS_OF_MONTHS_MM_DD|Example is 3/1.|
|THIRDS_OF_MONTHS_MM_DD_YY|Example is 3/1/10.|
|THIRDS_OF_MONTHS_MM_DDD|Examples are 3/B, 3/M, 3/E, 4/B|
|THIRDS_OF_MONTHS_MM_DDD_YY|Example is 3/B/10.|
|THIRDS_OF_MONTHS_MMM_DD|Examples are Mar 1, Mar 11, Mar 21, Apr 1|
|THIRDS_OF_MONTHS_MMM_DD_YY|Examples are Mar 1, '10; Mar 11, '10; Mar 21, '10; Apr 1, 10|
|THIRDS_OF_MONTHS_MMM_DDD|Examples are Mar B, Mar M, Mar E, Apr B|
|THIRDS_OF_MONTHS_MMM_DDD_YY|Examples are Mar B, '10; Mar M, '10; Mar E, '10; Apr B '10|
|THIRDS_OF_MONTHS_MMMM_DD|Examples are March 1, March 11, March 21, April 1|
|THIRDS_OF_MONTHS_MMMM_DD_YYYY|Examples are March 1, 2010; March 11, 2010; March 21, 2010; April 1, 2010|
|THIRDS_OF_MONTHS_MMMM_DDDD|Examples are March Beginning, March Middle, March End, April Beginning|
|THIRDS_OF_MONTHS_MMMM_DDDD_YYYY|Examples are March Beginning, 2010; March Middle, 2010; March End, 2010; April Beginning, 2010|
|WEEK_DDD_DD|Examples are Sun 21, Sun 28, Sun 4. Requires the time unit to be TimescaleWeeks.|
|WEEK_DDD_M_DD|Examples are Sun M 21, Sun M 28, Sun A 4|
|WEEK_DDD_MM_DD|Examples are Sun 3/21, Sun 3/28, Sun 4/4|
|WEEK_DDD_MM_DD_YY|Examples are Sun 3/21/10, Sun 3/28/10, Sun 4/4/10|
|WEEK_DDD_MMM_DD|Examples are Sun Mar 21, Sun Mar 28, Sun Apr 4|
|WEEK_DDD_MMM_DD_YYY|Examples are Sun Mar 21, '10; Sun Mar 28, '10; Sun Apr 4, '10|
|WEEK_DDD_MMMM_DD|Examples are Sun Mar 21, Sun March 28, Sun Apr 4|
|WEEK_DDD_MMMM_DD_YYY|Examples are Sun March 21, '10; Sun March 28, '10; Sun April 4, '10|
|WEEK_DDD_WW|Examples are Sun 12, Sun 13, Sun 14|
|WEEK_DDI_M_DD|Examples are Su M 21, Su M 28, Su A 4|
|WEEK_DDI_MM_DD|Examples are Su 3/21. Su 3/28, Su 4/4|
|WEEK_DDI_MMM_DD|Examples are Su Mar 21, Su Mar 28, Su Apr 4|
|WEEK_DI_M_DD|Examples are S M 21, S M 28, S A 4|
|WEEK_DI_MM_DD|Examples are S 3/21, S 3/28, S 4/4|
|WEEK_DI_MMM_DD|Examples are S Mar 21, S Mar 28, S Apr 4|
|WEEK_M_DD|Examples are M21, M28, A 4|
|WEEK_MM_DD|Examples are 3/21, 3/28, 4/4|
|WEEK_MM_DD_YY|Example is '3/21/10'.|
|WEEK_MMM_DD|Examples are Mar 21, Mar 28, Apr 4|
|WEEK_MMM_DD_YYY|Examples are Mar 21, '10; Mar 28, '10; Apr 4, '10|
|WEEK_MMMM_DD|Examples are March 21, March 28, April 4|
|WEEK_MMMM_DD_YYYY|Examples are March 21, 2010; March 28, 2010; April 4, 2010|
|WEEK_DAY_OF_MONTH_DD|Examples are 21, 28, 4|
|WEEK_FROM_END_WEEK_WW|Examples are Week 2, Week 1, Week -1 from the project end.|
|WEEK_FROM_END_WW|Examples are 2, 1, -1|
|WEEK_FROM_END_WWW|Examples are W2, W1, W-1|
|WEEK_FROM_START_WEEK_WW|Examples are Week -1, Week 1, Week 2 from the project start.|
|WEEK_FROM_START_WW|Examples are -1, 1, 2|
|WEEK_FROM_START_WWW|Examples are W-1, W1, W2|
|WEEK_NUMBER_DD_WW|Examples are 1 12, 1 13, 1 14 (day 1 of week 12, day 1 of week 13, and so forth)|
|WEEK_NUMBER_WW|Examples are 12, 13, 14|
|YEAR_YY|Examples are 10, 11, 12. Requires the time unit to be TimescaleYears.|
|YEAR_YYY|Examples are '10, '11, '12|
|YEAR_YYYY|Examples are 2010, 2011, 2012|
|YEAR_FROM_END_YEAR_YY|Examples are Year 2, Year 1, Year -1 from the project end.|
|YEAR_FROM_END_YY|Examples are 2, 1, -1|
|YEAR_FROM_END_YYY|Examples are Y2, Y1, Y-1|
|YEAR_FROM_START_YEAR_YY|Examples are Year -1, Year 1, Year 2 from the project start.|
|YEAR_FROM_START_YY|Examples are -1, 1, 2|
|YEAR_FROM_START_YYY|Examples are Y-1, Y1, Y2|

### See Also

* namespace [aspose.tasks.visualization](/tasks/python-net/aspose.tasks.visualization/)
* assembly [Aspose.Tasks](/tasks/python-net/)

