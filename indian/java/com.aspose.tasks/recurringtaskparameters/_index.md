---
title: "RecurringTaskParameters"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "एक प्रोजेक्ट में आवर्ती कार्य बनाने के लिए उपयोग किए जाने वाले पैरामीटर सेट का प्रतिनिधित्व करता है।"
type: docs
weight: 245
url: /hi/java/com.aspose.tasks/recurringtaskparameters/
---

**Inheritance:**
java.lang.Object
```
public class RecurringTaskParameters
```

एक प्रोजेक्ट में आवर्ती कार्य बनाने के लिए उपयोग किए जाने वाले पैरामीटर सेट का प्रतिनिधित्व करता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [RecurringTaskParameters()](#RecurringTaskParameters--) | एक नया उदाहरण प्रारंभ करता है [RecurringTaskParameters](../../com.aspose.tasks/recurringtaskparameters) क्लास का। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getDuration()](#getDuration--) | आवर्ती कार्य की एक घटना की अवधि प्राप्त करता है। |
| [getIgnoreResourceCalendar()](#getIgnoreResourceCalendar--) | एक मान प्राप्त करता है जो दर्शाता है कि क्या आवर्ती कार्य को तब भी शेड्यूल किया जाए जब कोई संसाधन उपलब्ध न हो। |
| [getRecurrencePattern()](#getRecurrencePattern--) | आवर्ती कार्य का पुनरावृत्ति पैटर्न प्राप्त करता है। |
| [getTaskName()](#getTaskName--) | आवर्ती कार्य का नाम प्राप्त करता है। |
| [setCalendar(Project project, String calendarName)](#setCalendar-com.aspose.tasks.Project-java.lang.String-) | आवर्ती कार्य के लिए कैलेंडर सेट करें। |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | पुनरावर्ती कार्य की एक घटना की अवधि निर्धारित करता है। |
| [setIgnoreResourceCalendar(boolean value)](#setIgnoreResourceCalendar-boolean-) | एक मान सेट करता है जो दर्शाता है कि क्या आवर्ती कार्य को तब भी शेड्यूल किया जाए जब कोई संसाधन उपलब्ध न हो। |
| [setRecurrencePattern(RecurrencePatternBase value)](#setRecurrencePattern-com.aspose.tasks.RecurrencePatternBase-) | आवर्ती कार्य का पुनरावृत्ति पैटर्न सेट करता है। |
| [setTaskName(String value)](#setTaskName-java.lang.String-) | आवर्ती कार्य का नाम सेट करता है। |
### RecurringTaskParameters() {#RecurringTaskParameters--}
```
public RecurringTaskParameters()
```


एक नया उदाहरण प्रारंभ करता है [RecurringTaskParameters](../../com.aspose.tasks/recurringtaskparameters) क्लास का।

### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


आवर्ती कार्य की एक घटना की अवधि प्राप्त करता है।

**Returns:**
[Duration](../../com.aspose.tasks/duration) - The instance of `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskparameters\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskparameters\#setDuration-Duration-)) class.
### getIgnoreResourceCalendar() {#getIgnoreResourceCalendar--}
```
public final boolean getIgnoreResourceCalendar()
```


एक मान प्राप्त करता है जो दर्शाता है कि क्या आवर्ती कार्य को तब भी शेड्यूल किया जाए जब कोई संसाधन उपलब्ध न हो।

**Returns:**
boolean - यह मान दर्शाता है कि क्या आवर्ती कार्य को तब भी शेड्यूल किया जाए जब कोई संसाधन उपलब्ध न हो कर उस पर काम किया जा सके।
### getRecurrencePattern() {#getRecurrencePattern--}
```
public final RecurrencePatternBase getRecurrencePattern()
```


आवर्ती कार्य का पुनरावृत्ति पैटर्न प्राप्त करता है।

--------------------

इनमें से एक मान हो सकता है `RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskparameters\#getRecurrencePattern--)/[setRecurrencePattern(RecurrencePatternBase)](../../com.aspose.tasks/recurringtaskparameters\#setRecurrencePattern-RecurrencePatternBase-)) एन्यूमरेशन।

**Returns:**
[RecurrencePatternBase](../../com.aspose.tasks/recurrencepatternbase) - the recurrence pattern of the recurring task.
### getTaskName() {#getTaskName--}
```
public final String getTaskName()
```


आवर्ती कार्य का नाम प्राप्त करता है।

**Returns:**
java.lang.String - आवर्ती कार्य का नाम।
### setCalendar(Project project, String calendarName) {#setCalendar-com.aspose.tasks.Project-java.lang.String-}
```
public final void setCalendar(Project project, String calendarName)
```


आवर्ती कार्य के लिए कैलेंडर सेट करें। कैलेंडर प्रोजेक्ट कैलेंडर संग्रह से चयनित किया जाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | कैलेंडर संग्रह वाला प्रोजेक्ट। |
| calendarName | java.lang.String | कैलेंडर का नाम। |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


पुनरावर्ती कार्य की एक घटना की अवधि निर्धारित करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskparameters\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskparameters\#setDuration-Duration-)) क्लास का इंस्टेंस। |

### setIgnoreResourceCalendar(boolean value) {#setIgnoreResourceCalendar-boolean-}
```
public final void setIgnoreResourceCalendar(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि क्या आवर्ती कार्य को तब भी शेड्यूल किया जाए जब कोई संसाधन उपलब्ध न हो।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि क्या आवर्ती कार्य को तब भी शेड्यूल किया जाए जब कोई संसाधन उपलब्ध न हो। |

### setRecurrencePattern(RecurrencePatternBase value) {#setRecurrencePattern-com.aspose.tasks.RecurrencePatternBase-}
```
public final void setRecurrencePattern(RecurrencePatternBase value)
```


आवर्ती कार्य का पुनरावृत्ति पैटर्न सेट करता है।

--------------------

इनमें से एक मान हो सकता है `RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskparameters\#getRecurrencePattern--)/[setRecurrencePattern(RecurrencePatternBase)](../../com.aspose.tasks/recurringtaskparameters\#setRecurrencePattern-RecurrencePatternBase-)) एन्यूमरेशन।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [RecurrencePatternBase](../../com.aspose.tasks/recurrencepatternbase) | आवर्ती कार्य का पुनरावृत्ति पैटर्न। |

### setTaskName(String value) {#setTaskName-java.lang.String-}
```
public final void setTaskName(String value)
```


आवर्ती कार्य का नाम सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | आवर्ती कार्य का नाम। |

