---
title: "ICalendar"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "तारीखों और अवधि की विभिन्न गणनाओं के लिए उपयोगी कैलेंडर एब्स्ट्रैक्शन का प्रतिनिधित्व करता है।"
type: docs
weight: 376
url: /hi/java/com.aspose.tasks/icalendar/
---
```
public interface ICalendar
```

तारीखों और अवधि की विभिन्न गणनाओं के लिए उपयोगी कैलेंडर एब्स्ट्रैक्शन का प्रतिनिधित्व करता है।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getFinishDateByStartAndWork(Date start, Duration work)](#getFinishDateByStartAndWork-java.util.Date-com.aspose.tasks.Duration-) | कैलेंडर के अनुसार निर्दिष्ट कार्य समय की मात्रा समाप्त होने की तिथि की गणना करता है. |
| [getFinishDateByStartAndWork(Date start, double work)](#getFinishDateByStartAndWork-java.util.Date-double-) | कैलेंडर के अनुसार निर्दिष्ट कार्य समय की मात्रा समाप्त होने की तिथि की गणना करता है. |
| [getNextWorkingDayStart(Date date)](#getNextWorkingDayStart-java.util.Date-) | निर्दिष्ट तिथि के लिए अगले कार्य दिवस की शुरुआत की गणना करता है. |
| [getPreviousWorkingDayEnd(Date date)](#getPreviousWorkingDayEnd-java.util.Date-) | निर्दिष्ट तिथि से पिछले कार्य दिवस का अंत गणना करता है. |
| [getStartDateFromFinishAndDuration(Date finish, Duration duration)](#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-) | निर्दिष्ट समाप्ति तिथि और अवधि के आधार पर प्रारंभ तिथि लौटाता है. |
| [getStartDateFromFinishAndDuration(Date finish, double duration)](#getStartDateFromFinishAndDuration-java.util.Date-double-) | निर्दिष्ट समाप्ति तिथि और अवधि के आधार पर प्रारंभ तिथि लौटाता है. |
| [getTaskFinishDateFromDuration(Task task, double duration)](#getTaskFinishDateFromDuration-com.aspose.tasks.Task-double-) | कार्य की प्रारंभ तिथि, विभाजित भाग और कार्य अवधि से समाप्ति तिथि और समय की गणना करता है. |
| [getWorkStart(Date date)](#getWorkStart-java.util.Date-) | निर्दिष्ट तिथि और समय से शुरू होकर अगले कार्य समय की शुरुआत की गणना करता है. |
| [getWorkingHours(Date dt)](#getWorkingHours-java.util.Date-) | निर्दिष्ट तिथि पर कार्य घंटों की मात्रा लौटाता है. |
| [getWorkingHours(Date start, Date finish)](#getWorkingHours-java.util.Date-java.util.Date-) | WorkUnit लौटाता है - निर्दिष्ट तिथि‑समय अंतराल के लिए कार्य घंटों की प्रारंभ, समाप्ति और अवधि. |
| [getWorkingHoursTimeSpan(Date start, Date finish)](#getWorkingHoursTimeSpan-java.util.Date-java.util.Date-) | निर्दिष्ट तिथियों के बीच कार्य घंटों की मात्रा लौटाता है. |
| [getWorkingTimes(Date dt)](#getWorkingTimes-java.util.Date-) | निर्दिष्ट तिथि के लिए कार्य समय की [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) लौटाता है. |
| [isDayWorking(Date dt)](#isDayWorking-java.util.Date-) | कैलेंडर के अनुसार निर्धारित करता है कि निर्दिष्ट दिन कार्य दिवस है या नहीं. |
| [isEmpty()](#isEmpty--) | लौटाता है कि कैलेंडर में कार्य घंटे परिभाषित नहीं हैं या नहीं. |
### getFinishDateByStartAndWork(Date start, Duration work) {#getFinishDateByStartAndWork-java.util.Date-com.aspose.tasks.Duration-}
```
public abstract Date getFinishDateByStartAndWork(Date start, Duration work)
```


कैलेंडर के अनुसार निर्दिष्ट कार्य समय की मात्रा समाप्त होने की तिथि की गणना करता है.

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रारंभ | java.util.Date | प्रारम्भ तिथि. |
| work | [Duration](../../com.aspose.tasks/duration) | कार्य अवधि. |

**Returns:**
java.util.Date - समाप्ति तिथि.
### getFinishDateByStartAndWork(Date start, double work) {#getFinishDateByStartAndWork-java.util.Date-double-}
```
public abstract Date getFinishDateByStartAndWork(Date start, double work)
```


कैलेंडर के अनुसार निर्दिष्ट कार्य समय की मात्रा समाप्त होने की तिथि की गणना करता है.

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रारंभ | java.util.Date | प्रारम्भ तिथि. |
| कार्य | double | कार्य अवधि. |

**Returns:**
java.util.Date - समाप्ति तिथि.
### getNextWorkingDayStart(Date date) {#getNextWorkingDayStart-java.util.Date-}
```
public abstract Date getNextWorkingDayStart(Date date)
```


निर्दिष्ट तिथि के लिए अगले कार्य दिवस की शुरुआत की गणना करता है.

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| तारीख | java.util.Date | अगले कार्य दिवस की शुरुआत प्राप्त करने के लिए तारीख। |

**Returns:**
java.util.Date - अगले कार्य दिवस की शुरुआत System.DateTime।
### getPreviousWorkingDayEnd(Date date) {#getPreviousWorkingDayEnd-java.util.Date-}
```
public abstract Date getPreviousWorkingDayEnd(Date date)
```


निर्दिष्ट तिथि से पिछले कार्य दिवस का अंत गणना करता है.

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| तारीख | java.util.Date | पिछले कार्य दिवस के अंत की गणना करने के लिए तारीख। |

**Returns:**
java.util.Date - पिछले कार्य दिवस के अंत का अंत
### getStartDateFromFinishAndDuration(Date finish, Duration duration) {#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-}
```
public abstract Date getStartDateFromFinishAndDuration(Date finish, Duration duration)
```


निर्दिष्ट समाप्ति तिथि और अवधि के आधार पर प्रारंभ तिथि लौटाता है.

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| समाप्ति | java.util.Date | निर्दिष्ट समाप्ति तारीख। |
| duration | [Duration](../../com.aspose.tasks/duration) | निर्दिष्ट अवधि। |

**Returns:**
java.util.Date - गणना की गई प्रारंभिक तारीख।
### getStartDateFromFinishAndDuration(Date finish, double duration) {#getStartDateFromFinishAndDuration-java.util.Date-double-}
```
public abstract Date getStartDateFromFinishAndDuration(Date finish, double duration)
```


निर्दिष्ट समाप्ति तिथि और अवधि के आधार पर प्रारंभ तिथि लौटाता है.

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| समाप्ति | java.util.Date | निर्दिष्ट समाप्ति तारीख। |
| अवधि | double | निर्दिष्ट अवधि। |

**Returns:**
java.util.Date - गणना की गई प्रारंभिक तारीख।
### getTaskFinishDateFromDuration(Task task, double duration) {#getTaskFinishDateFromDuration-com.aspose.tasks.Task-double-}
```
public abstract Date getTaskFinishDateFromDuration(Task task, double duration)
```


कार्य की प्रारंभ तिथि, विभाजित भाग और कार्य अवधि से समाप्ति तिथि और समय की गणना करता है.

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | समाप्ति तारीख की गणना करने के लिए कार्य। |
|  | अवधि | double | गणना करने के लिए अवधि। |

यदि कार्य सारांश है, null है या उसकी प्रारंभिक तारीख सेट नहीं है तो DateTime.MinValue लौटाता है। |

**Returns:**
java.util.Date - दिए गए प्रारंभिक तारीख और अवधि के लिए कार्य की समाप्ति तारीख।
### getWorkStart(Date date) {#getWorkStart-java.util.Date-}
```
public abstract Date getWorkStart(Date date)
```


निर्दिष्ट तिथि और समय से शुरू होकर अगले कार्य समय की शुरुआत की गणना करता है.

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| तारीख | java.util.Date | तारीख और समय। |

**Returns:**
java.util.Date - निकटतम कार्य समय की शुरुआत।
### getWorkingHours(Date dt) {#getWorkingHours-java.util.Date-}
```
public abstract double getWorkingHours(Date dt)
```


निर्दिष्ट तिथि पर कार्य घंटों की मात्रा लौटाता है.

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| dt | java.util.Date | कार्य घंटे प्राप्त करने के लिए तारीख। |

**Returns:**
double - निर्दिष्ट तारीख पर कार्य घंटे।
### getWorkingHours(Date start, Date finish) {#getWorkingHours-java.util.Date-java.util.Date-}
```
public abstract WorkUnit getWorkingHours(Date start, Date finish)
```


WorkUnit लौटाता है - निर्दिष्ट तिथि‑समय अंतराल के लिए कार्य घंटों की प्रारंभ, समाप्ति और अवधि.

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रारंभ | java.util.Date | अंतराल की प्रारंभिक तारीख। |
| समाप्ति | java.util.Date | अंतराल की समाप्ति तारीख। |

**Returns:**
[WorkUnit](../../com.aspose.tasks/workunit) - Instance of [WorkUnit](../../com.aspose.tasks/workunit) class containing Start, Finish and Duration of working hours.
### getWorkingHoursTimeSpan(Date start, Date finish) {#getWorkingHoursTimeSpan-java.util.Date-java.util.Date-}
```
public abstract double getWorkingHoursTimeSpan(Date start, Date finish)
```


निर्दिष्ट तिथियों के बीच कार्य घंटों की मात्रा लौटाता है.

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रारंभ | java.util.Date | अंतराल की प्रारंभिक तारीख। |
| समाप्ति | java.util.Date | अंतराल की समाप्ति तारीख। |

**Returns:**
double - कैलेंडर इंस्टेंस के अनुसार कार्य घंटों की मात्रा।
### getWorkingTimes(Date dt) {#getWorkingTimes-java.util.Date-}
```
public abstract WorkingTimeCollection getWorkingTimes(Date dt)
```


निर्दिष्ट तिथि के लिए कार्य समय की [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) लौटाता है.

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| dt | java.util.Date | कार्य समय प्राप्त करने के लिए तारीख। |

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - Collection of [WorkingTime](../../com.aspose.tasks/workingtime) instances.
### isDayWorking(Date dt) {#isDayWorking-java.util.Date-}
```
public abstract boolean isDayWorking(Date dt)
```


कैलेंडर के अनुसार निर्धारित करता है कि निर्दिष्ट दिन कार्य दिवस है या नहीं.

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| dt | java.util.Date | जाँचने के लिए कि दिन कार्य दिवस है या नहीं, तारीख। |

**Returns:**
boolean - यदि दिन कार्य दिवस है तो सत्य।
### isEmpty() {#isEmpty--}
```
public abstract boolean isEmpty()
```


लौटाता है कि कैलेंडर में कार्य घंटे परिभाषित नहीं हैं या नहीं.

**Returns:**
boolean - यदि कैलेंडर में कार्य घंटे परिभाषित नहीं हैं तो सही।
