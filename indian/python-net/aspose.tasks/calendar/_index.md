---
title: "Calendar"
second_title: "Aspose.Tasks Python के लिए .NET API संदर्भ"
description: 
type: docs
weight: 140
url: /hi/python-net/aspose.tasks/calendar/
---

## Calendar class

प्रोजेक्ट में उपयोग किए जाने वाले कैलेंडर का प्रतिनिधित्व करता है।

Calendar प्रकार निम्नलिखित सदस्यों को उजागर करता है:
## गुणधर्म
| नाम | विवरण |
| :- | :- |
| name | कैलेंडर का नाम प्राप्त करता है या सेट करता है। |
| uid | कैलेंडर की विशिष्ट पहचानकर्ता को प्राप्त करता है या सेट करता है। |
| week_days | इस कैलेंडर के लिए WeekDaysCollection प्राप्त करता है।<br/>            कैलेंडर को परिभाषित करने वाले सप्ताह के दिनों का संग्रह। |
| exceptions | CalendarExceptionCollection ऑब्जेक्ट प्राप्त करता है।<br/>            कैलेंडर से संबंधित अपवादों का संग्रह। |
| work_weeks | WorkWeekCollections ऑब्जेक्ट प्राप्त करता है।<br/>            कैलेंडर से संबंधित कार्य सप्ताहों का संग्रह। |
| is_base_calendar | यह दर्शाने वाला मान प्राप्त करता है कि कैलेंडर बेस कैलेंडर है या नहीं। |
| base_calendar | इस कैलेंडर पर निर्भर बेस कैलेंडर को प्राप्त करता है या सेट करता है।<br/>            केवल तब लागू जब कैलेंडर बेस कैलेंडर न हो। |
| is_baseline_calendar | कैलेंडर बेसलाइन कैलेंडर है या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है। |
| guid | कैलेंडर का Guid प्राप्त करता है। |
| प्रिमावेरा_प्रॉपर्टीज़ | Primavera फ़ॉर्मैट से पढ़े गए कैलेंडर के लिए Primavera-विशिष्ट गुणों वाला ऑब्जेक्ट प्राप्त करता है। |
## Methods
| नाम | विवरण |
| :- | :- |
| get_start_date_from_finish_and_duration(finish, duration) | निर्दिष्ट समाप्ति तिथि और अवधि के आधार पर प्रारंभ तिथि लौटाता है। |
| get_start_date_from_finish_and_duration(finish, duration) | निर्दिष्ट समाप्ति तिथि और अवधि के आधार पर प्रारंभ तिथि लौटाता है। |
| get_working_hours(start, finish) | निर्दिष्ट तिथि-समय अंतराल के लिए कार्य घंटे की शुरुआत, समाप्ति और अवधि वाला WorkUnit लौटाता है। |
| get_working_hours(dt) | निर्दिष्ट तिथि-समय अंतराल के लिए कार्य घंटे की शुरुआत, समाप्ति और अवधि वाला WorkUnit लौटाता है। |
| get_finish_date_by_start_and_work(start, work) | कैलेंडर के अनुसार निर्दिष्ट कार्य समय की मात्रा के समाप्त होने की तिथि की गणना करता है। |
| get_finish_date_by_start_and_work(start, work) | कैलेंडर के अनुसार निर्दिष्ट कार्य समय की मात्रा के समाप्त होने की तिथि की गणना करता है। |
| get_intersection_calendar(calendar1, calendar2) | 2 कैलेंडरों के कार्य शेड्यूल के प्रतिच्छेदन पर गणनाएँ करने के लिए उपयोग किया जा सकने वाला [ICalendar](/tasks/python-net/aspose.tasks/icalendar/) इंस्टेंस प्राप्त करता है। |
| make_standard_calendar(calendar) | डिफ़ॉल्ट मानक कैलेंडर बनाता है। |
| make_24_hour_calendar(calendar) | दिए गए कैलेंडर को 24Hour Calendar बनाता है।<br/>            24Hours Calendar वह कैलेंडर है जिसमें सप्ताह के हर दिन लगातार कार्य घंटे के साथ काम करता है। |
| make_night_shift_calendar(calendar) | दिए गए कैलेंडर को Night Shift Calendar बनाता है। |
| delete() | परियोजना से कैलेंडर हटाता है। |
| is_day_working(dt) | कैलेंडर के अनुसार निर्धारित करता है कि निर्दिष्ट दिन कार्य दिवस है या नहीं। |
| get_working_hours_time_span(start, finish) | निर्दिष्ट तिथियों के बीच कार्य घंटों की मात्रा लौटाता है। |
| get_task_finish_date_from_duration(task, duration) | कार्य की प्रारंभ तिथि, विभाजित भागों और कार्य अवधि से समाप्ति तिथि और समय की गणना करता है। |
| get_working_times(dt) | निर्दिष्ट तिथि के लिए कार्य समय की [WorkingTimeCollection](/tasks/python-net/aspose.tasks/workingtimecollection/) लौटाता है। |
| get_previous_working_day_end(date) | निर्दिष्ट तिथि से पिछले कार्य तिथि का अंत गणना करता है। |
| get_next_working_day_start(date) | निर्दिष्ट तिथि के लिए अगले कार्य दिवस की शुरुआत की गणना करता है। |
| get_work_start(date) | निर्दिष्ट तिथि और समय से शुरू होकर अगले कार्य समय की शुरुआत की गणना करता है। |
| is_empty() | लौटाता है कि क्या कैलेंडर में कार्य घंटे परिभाषित नहीं हैं। |

### संबंधित देखें

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

