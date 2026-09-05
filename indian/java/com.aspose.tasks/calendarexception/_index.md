---
title: "CalendarException"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "कैलेंडर में असाधारण समय अवधि को दर्शाता है।"
type: docs
weight: 43
url: /hi/java/com.aspose.tasks/calendarexception/
---

**Inheritance:**
java.lang.Object
```
public final class CalendarException
```

कैलेंडर में असाधारण समय अवधि को दर्शाता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [CalendarException()](#CalendarException--) | नया उदाहरण प्रारंभ करता है [CalendarException](../../com.aspose/tasks/calendarexception) क्लास का। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [checkException(Date dt)](#checkException-java.util.Date-) | सही लौटाता है यदि निर्दिष्ट java.util.Date स्ट्रक्चर का उदाहरण अपवाद दिन है। |
| [delete()](#delete--) | पैरेंट कैलेंडर CalendarExceptionCollection ऑब्जेक्ट से Exception उदाहरण को हटाता है। |
| [getDayWorking()](#getDayWorking--) | एक मान प्राप्त करता है जो दर्शाता है कि निर्दिष्ट तिथि या दिन प्रकार कार्यशील है या नहीं। |
| [getDaysOfWeek()](#getDaysOfWeek--) | इस ऑब्जेक्ट के लिए DayTypeCollection प्राप्त करता है। |
| [getEnteredByOccurrences()](#getEnteredByOccurrences--) | एक मान प्राप्त करता है जो दर्शाता है कि क्या पुनरावृत्ति की सीमा घटनाओं की संख्या दर्ज करके परिभाषित की गई है। |
| [getExceptionDates()](#getExceptionDates--) | उन तिथियों को लौटाता है जिन पर कैलेंडर अपवाद लागू होता है। |
| [getFromDate()](#getFromDate--) | अपवाद समय की शुरुआत प्राप्त करता है। |
| [getMonth()](#getMonth--) | उस महीने को प्राप्त करता है जिसके लिए अपवाद पुनरावृत्ति निर्धारित है। |
| [getMonthDay()](#getMonthDay--) | उस महीने के दिन को प्राप्त करता है जिस पर अपवाद पुनरावृत्ति निर्धारित है। |
| [getMonthItem()](#getMonthItem--) | उस महीने के आइटम को प्राप्त करता है जिसके लिए अपवाद पुनरावृत्ति निर्धारित है। |
| [getMonthPosition()](#getMonthPosition--) | एक महीने के भीतर महीने के आइटम की स्थिति प्राप्त करता है। |
| [getName()](#getName--) | अपवाद का नाम प्राप्त करता है। |
| [getOccurrences()](#getOccurrences--) | कैलेंडर अपवाद के वैध होने के लिए घटनाओं की संख्या प्राप्त करता है। |
| [getParentCalendar()](#getParentCalendar--) | इस ऑब्जेक्ट के लिए पैरेंट कैलेंडर प्राप्त करता है। |
| [getPeriod()](#getPeriod--) | अपवाद के लिए पुनरावृत्ति की अवधि प्राप्त करता है। |
| [getToDate()](#getToDate--) | अपवाद समय का अंत प्राप्त करता है। |
| [getType()](#getType--) | अपवाद प्रकार प्राप्त करता है। |
| [getWorkingTime()](#getWorkingTime--) | कैलेंडर अपवाद के लिए कार्य समय लौटाता है। |
| [getWorkingTimes()](#getWorkingTimes--) | WorkingTimeCollection ऑब्जेक्ट प्राप्त करता है। |
| [setDayWorking(boolean value)](#setDayWorking-boolean-) | एक मान सेट करता है जो दर्शाता है कि निर्दिष्ट तिथि या दिन प्रकार कार्यशील है या नहीं। |
| [setEnteredByOccurrences(boolean value)](#setEnteredByOccurrences-boolean-) | एक मान सेट करता है जो दर्शाता है कि क्या पुनरावृत्ति की सीमा घटनाओं की संख्या दर्ज करके परिभाषित की गई है। |
| [setFromDate(Date value)](#setFromDate-java.util.Date-) | अपवाद समय की शुरुआत सेट करता है। |
| [setMonth(int value)](#setMonth-int-) | उस महीने को सेट करता है जिसके लिए अपवाद आवृत्ति निर्धारित है। |
| [setMonthDay(int value)](#setMonthDay-int-) | उस महीने के दिन को सेट करता है जिस पर अपवाद आवृत्ति निर्धारित है। |
| [setMonthItem(int value)](#setMonthItem-int-) | उस महीने के आइटम को सेट करता है जिसके लिए अपवाद आवृत्ति निर्धारित है। |
| [setMonthPosition(int value)](#setMonthPosition-int-) | महीने के भीतर महीने के आइटम की स्थिति सेट करता है। |
| [setName(String value)](#setName-java.lang.String-) | अपवाद का नाम सेट करता है। |
| [setOccurrences(int value)](#setOccurrences-int-) | कैलेंडर अपवाद के वैध होने की घटनाओं की संख्या सेट करता है। |
| [setPeriod(int value)](#setPeriod-int-) | अपवाद के लिए आवृत्ति अवधि सेट करता है। |
| [setToDate(Date value)](#setToDate-java.util.Date-) | अपवाद समय का अंत सेट करता है। |
| [setType(int value)](#setType-int-) | अपवाद प्रकार सेट करता है। |
| [setWorkingTimes(WorkingTimeCollection value)](#setWorkingTimes-com.aspose.tasks.WorkingTimeCollection-) | WorkingTimeCollection ऑब्जेक्ट सेट करता है। |
### CalendarException() {#CalendarException--}
```
public CalendarException()
```


नया उदाहरण प्रारंभ करता है [CalendarException](../../com.aspose/tasks/calendarexception) क्लास का।

### checkException(Date dt) {#checkException-java.util.Date-}
```
public final boolean checkException(Date dt)
```


सही लौटाता है यदि निर्दिष्ट java.util.Date स्ट्रक्चर का उदाहरण अपवाद दिन है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| dt | java.util.Date | java.util.Date स्ट्रक्ट का निर्दिष्ट उदाहरण। |

**Returns:**
boolean - यदि java.util.Date मान अपवाद दिवस है तो true लौटाता है; अन्यथा false।
### delete() {#delete--}
```
public final void delete()
```


पैरेंट कैलेंडर CalendarExceptionCollection ऑब्जेक्ट से Exception उदाहरण को हटाता है।

### getDayWorking() {#getDayWorking--}
```
public final boolean getDayWorking()
```


एक मान प्राप्त करता है जो दर्शाता है कि निर्दिष्ट तिथि या दिन प्रकार कार्यशील है या नहीं।

**Returns:**
boolean - एक मान जो दर्शाता है कि निर्दिष्ट तिथि या दिन प्रकार कार्यशील है या नहीं।
### getDaysOfWeek() {#getDaysOfWeek--}
```
public final DayTypeCollection getDaysOfWeek()
```


इस ऑब्जेक्ट के लिए DayTypeCollection प्राप्त करता है। वह सप्ताह के दिन जिन पर अपवाद वैध है।

**Returns:**
[DayTypeCollection](../../com.aspose.tasks/daytypecollection) - the DayTypeCollection for this object.
### getEnteredByOccurrences() {#getEnteredByOccurrences--}
```
public final boolean getEnteredByOccurrences()
```


एक मान प्राप्त करता है जो दर्शाता है कि क्या आवृत्ति की सीमा घटनाओं की संख्या दर्ज करके परिभाषित की गई है। False यह निर्दिष्ट करता है कि आवृत्ति की सीमा समाप्ति तिथि दर्ज करके परिभाषित की गई है।

**Returns:**
boolean - एक मान जो दर्शाता है कि क्या आवृत्ति की सीमा घटनाओं की संख्या दर्ज करके परिभाषित की गई है।
### getExceptionDates() {#getExceptionDates--}
```
public final Iterable<Date> getExceptionDates()
```


उन तिथियों को लौटाता है जिन पर कैलेंडर अपवाद लागू होता है।

**Returns:**
java.lang.Iterable&lt;java.util.Date&gt; - वे तिथियां जिन पर कैलेंडर अपवाद लागू होता है।
### getFromDate() {#getFromDate--}
```
public final Date getFromDate()
```


अपवाद समय की शुरुआत प्राप्त करता है।

**Returns:**
java.util.Date - अपवाद समय की शुरुआत।
### getMonth() {#getMonth--}
```
public final int getMonth()
```


उस महीने को प्राप्त करता है जिसके लिए अपवाद पुनरावृत्ति निर्धारित है।

**Returns:**
int - वह महीना जिसके लिए अपवाद आवृत्ति निर्धारित है।
### getMonthDay() {#getMonthDay--}
```
public final int getMonthDay()
```


उस महीने के दिन को प्राप्त करता है जिस पर अपवाद पुनरावृत्ति निर्धारित है।

**Returns:**
int - वह महीने का दिन जिस पर अपवाद आवृत्ति निर्धारित है।
### getMonthItem() {#getMonthItem--}
```
public final int getMonthItem()
```


उस महीने के आइटम को प्राप्त करता है जिसके लिए अपवाद पुनरावृत्ति निर्धारित है।

**Returns:**
int - वह महीने का आइटम जिसके लिए अपवाद आवृत्ति निर्धारित है।
### getMonthPosition() {#getMonthPosition--}
```
public final int getMonthPosition()
```


एक महीने के भीतर महीने के आइटम की स्थिति प्राप्त करता है।

**Returns:**
int - महीने के भीतर महीने के आइटम की स्थिति।
### getName() {#getName--}
```
public final String getName()
```


अपवाद का नाम प्राप्त करता है।

**Returns:**
java.lang.String - अपवाद का नाम।
### getOccurrences() {#getOccurrences--}
```
public final int getOccurrences()
```


कैलेंडर अपवाद के वैध होने के लिए घटनाओं की संख्या प्राप्त करता है।

**Returns:**
int - वह घटनाओं की संख्या जिसके लिए कैलेंडर अपवाद वैध है।
### getParentCalendar() {#getParentCalendar--}
```
public final Calendar getParentCalendar()
```


इस ऑब्जेक्ट के लिए पैरेंट कैलेंडर प्राप्त करता है।

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - the parent calendar for this object.
### getPeriod() {#getPeriod--}
```
public final int getPeriod()
```


अपवाद के लिए पुनरावृत्ति की अवधि प्राप्त करता है।

**Returns:**
int - अपवाद के लिए आवृत्ति अवधि।
### getToDate() {#getToDate--}
```
public final Date getToDate()
```


अपवाद समय का अंत प्राप्त करता है।

**Returns:**
java.util.Date - अपवाद समय का अंत।
### getType() {#getType--}
```
public final int getType()
```


अपवाद प्रकार प्राप्त करता है।

**Returns:**
int - अपवाद प्रकार।
### getWorkingTime() {#getWorkingTime--}
```
public final double getWorkingTime()
```


कैलेंडर अपवाद के लिए कार्य समय लौटाता है।

**Returns:**
double - इस कैलेंडर अपवाद के लिए कार्य समय लौटाता है।
### getWorkingTimes() {#getWorkingTimes--}
```
public final WorkingTimeCollection getWorkingTimes()
```


WorkingTimeCollection ऑब्जेक्ट प्राप्त करता है। कार्यदिवस पर काम किए गए समय को परिभाषित करने वाले कार्य समय का संग्रह।

--------------------

कम से कम एक कार्य समय मौजूद होना चाहिए, और अधिकतम पाँच से अधिक नहीं हो सकता।

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - the WorkingTimeCollection object.
### setDayWorking(boolean value) {#setDayWorking-boolean-}
```
public final void setDayWorking(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि निर्दिष्ट तिथि या दिन प्रकार कार्यशील है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि निर्दिष्ट तिथि या दिन प्रकार कार्यशील है या नहीं। |

### setEnteredByOccurrences(boolean value) {#setEnteredByOccurrences-boolean-}
```
public final void setEnteredByOccurrences(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि आवृत्ति की सीमा घटनाओं की संख्या दर्ज करके परिभाषित है या नहीं। False यह निर्दिष्ट करता है कि आवृत्ति की सीमा समाप्ति तिथि दर्ज करके परिभाषित है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि आवृत्ति की सीमा घटनाओं की संख्या दर्ज करके परिभाषित है। |

### setFromDate(Date value) {#setFromDate-java.util.Date-}
```
public final void setFromDate(Date value)
```


अपवाद समय की शुरुआत सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.Date | अपवाद समय की शुरुआत। |

### setMonth(int value) {#setMonth-int-}
```
public final void setMonth(int value)
```


उस महीने को सेट करता है जिसके लिए अपवाद आवृत्ति निर्धारित है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | वह महीना जिसके लिए अपवाद आवृत्ति निर्धारित है। |

### setMonthDay(int value) {#setMonthDay-int-}
```
public final void setMonthDay(int value)
```


उस महीने के दिन को सेट करता है जिस पर अपवाद आवृत्ति निर्धारित है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | वह दिन जिसका महीना में अपवाद आवृत्ति निर्धारित है। |

### setMonthItem(int value) {#setMonthItem-int-}
```
public final void setMonthItem(int value)
```


उस महीने के आइटम को सेट करता है जिसके लिए अपवाद आवृत्ति निर्धारित है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | वह महीना आइटम जिसके लिए अपवाद आवृत्ति निर्धारित है। |

### setMonthPosition(int value) {#setMonthPosition-int-}
```
public final void setMonthPosition(int value)
```


महीने के भीतर महीने के आइटम की स्थिति सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | महीने के भीतर महीने आइटम की स्थिति। |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


अपवाद का नाम सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | अपवाद का नाम। |

### setOccurrences(int value) {#setOccurrences-int-}
```
public final void setOccurrences(int value)
```


कैलेंडर अपवाद के वैध होने की घटनाओं की संख्या सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | कैलेंडर अपवाद के वैध होने की घटनाओं की संख्या। |

### setPeriod(int value) {#setPeriod-int-}
```
public final void setPeriod(int value)
```


अपवाद के लिए आवृत्ति अवधि सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | अपवाद की आवृत्ति अवधि। |

### setToDate(Date value) {#setToDate-java.util.Date-}
```
public final void setToDate(Date value)
```


अपवाद समय का अंत सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.Date | अपवाद समय का अंत। |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


अपवाद प्रकार सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | अपवाद प्रकार। |

### setWorkingTimes(WorkingTimeCollection value) {#setWorkingTimes-com.aspose.tasks.WorkingTimeCollection-}
```
public final void setWorkingTimes(WorkingTimeCollection value)
```


WorkingTimeCollection ऑब्जेक्ट सेट करता है। कार्यदिवस पर काम किए गए समय को परिभाषित करने वाले कार्य समय का संग्रह।

--------------------

कम से कम एक कार्य समय मौजूद होना चाहिए, और अधिकतम पाँच से अधिक नहीं हो सकता।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) | WorkingTimeCollection ऑब्जेक्ट। |

