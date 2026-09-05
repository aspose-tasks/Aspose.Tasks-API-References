---
title: "WeekDay"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "एक सप्ताह का दिन दर्शाता है जो या तो कैलेंडर में नियमित दिनों या अपवाद दिनों को परिभाषित करता है।"
type: docs
weight: 352
url: /hi/java/com.aspose.tasks/weekday/
---

**Inheritance:**
java.lang.Object
```
public class WeekDay
```

एक सप्ताह का दिन दर्शाता है जो या तो कैलेंडर में नियमित दिनों या अपवाद दिनों को परिभाषित करता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [WeekDay(int dayType)](#WeekDay-int-) | निर्दिष्ट दिन प्रकार के साथ [WeekDay](../../com.aspose/tasks/weekday) क्लास का नया उदाहरण प्रारंभ करता है। |
| [WeekDay(int dayType, List&lt;WorkingTime&gt; workingTimes)](#WeekDay-int-java.util.List-com.aspose.tasks.WorkingTime--) | निर्दिष्ट दिन प्रकार और कार्य समय अवधि की सूची के साथ [WeekDay](../../com.aspose/tasks/weekday) क्लास का नया उदाहरण प्रारंभ करता है। |
| [WeekDay(int dayType, WorkingTime[] workingTimes)](#WeekDay-int-com.aspose.tasks.WorkingTime...-) | निर्दिष्ट दिन प्रकार और कार्य समय अवधि के साथ [WeekDay](../../com.aspose/tasks/weekday) क्लास का नया उदाहरण प्रारंभ करता है। |
| [WeekDay()](#WeekDay--) | नया उदाहरण प्रारंभ करता है [WeekDay](../../com.aspose.tasks/weekday) वर्ग का। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [castToDayType(int dw)](#castToDayType-int-) | .Net के [DayOfWeek](../../com.aspose.tasks/dayofweek) को `DayType`([getDayType()](../../com.aspose.tasks/weekday\#getDayType--)/[setDayType(int)](../../com.aspose.tasks/weekday\#setDayType-int-)) में कास्ट करता है। |
| [createDefaultWorkingDay(int dayType)](#createDefaultWorkingDay-int-) | डिफ़ॉल्ट कार्य दिवस बनाता है। |
| [deepClone()](#deepClone--) | सप्ताह के दिन की गहरी कॉपी लौटाता है। |
| [equals(Object obj)](#equals-java.lang.Object-) | एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| [getDayType()](#getDayType--) | एक दिन का प्रकार प्राप्त करता है। |
| [getDayWorking()](#getDayWorking--) | एक मान प्राप्त करता है जो दर्शाता है कि निर्दिष्ट तिथि या दिन प्रकार कार्यशील है या नहीं। |
| [getFromDate()](#getFromDate--) | एक अपवाद समय की शुरुआत प्राप्त करता है। |
| [getToDate()](#getToDate--) | एक अपवाद समय का अंत प्राप्त करता है। |
| [getWorkingTime()](#getWorkingTime--) | सप्ताह के दिन के लिए कार्य समय लौटाता है। |
| [getWorkingTimes()](#getWorkingTimes--) | इस WeekDay उदाहरण के लिए WorkingTimeCollection प्राप्त करता है। |
| [hashCode()](#hashCode--) | [WeekDay](../../com.aspose.tasks/weekday) वर्ग के उदाहरण के लिए हैश कोड मान लौटाता है। |
| [setDayWorking(boolean value)](#setDayWorking-boolean-) | एक मान सेट करता है जो दर्शाता है कि निर्दिष्ट तिथि या दिन प्रकार कार्यशील है या नहीं। |
| [setDefaultWorkingTime(WeekDay day)](#setDefaultWorkingTime-com.aspose.tasks.WeekDay-) | निर्दिष्ट सप्ताह के दिन के लिए डिफ़ॉल्ट समय अवधि सेट करता है। |
| [setFromDate(Date value)](#setFromDate-java.util.Date-) | एक अपवाद समय की शुरुआत सेट करता है। |
| [setToDate(Date value)](#setToDate-java.util.Date-) | एक अपवाद समय का अंत सेट करता है। |
### WeekDay(int dayType) {#WeekDay-int-}
```
public WeekDay(int dayType)
```


निर्दिष्ट दिन प्रकार के साथ [WeekDay](../../com.aspose/tasks/weekday) क्लास का नया उदाहरण प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| dayType | int | निर्दिष्ट दिन प्रकार। |

### WeekDay(int dayType, List&lt;WorkingTime&gt; workingTimes) {#WeekDay-int-java.util.List-com.aspose.tasks.WorkingTime--}
```
public WeekDay(int dayType, List<WorkingTime> workingTimes)
```


निर्दिष्ट दिन प्रकार और कार्य समय अवधि की सूची के साथ [WeekDay](../../com.aspose/tasks/weekday) क्लास का नया उदाहरण प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| dayType | int | निर्दिष्ट दिन प्रकार। |
| workingTimes | java.util.List&lt;com.aspose.tasks.WorkingTime&gt; | कार्य समय अवधि की सूची। |

### WeekDay(int dayType, WorkingTime[] workingTimes) {#WeekDay-int-com.aspose.tasks.WorkingTime...-}
```
public WeekDay(int dayType, WorkingTime[] workingTimes)
```


निर्दिष्ट दिन प्रकार और कार्य समय अवधि के साथ [WeekDay](../../com.aspose/tasks/weekday) क्लास का नया उदाहरण प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| dayType | int | निर्दिष्ट दिन प्रकार। |
| workingTimes | [WorkingTime\[\]](../../com.aspose.tasks/workingtime) | कार्य समय अवधि का एरे। |

### WeekDay() {#WeekDay--}
```
public WeekDay()
```


नया उदाहरण प्रारंभ करता है [WeekDay](../../com.aspose.tasks/weekday) वर्ग का।

### castToDayType(int dw) {#castToDayType-int-}
```
public static int castToDayType(int dw)
```


.Net के [DayOfWeek](../../com.aspose.tasks/dayofweek) को `DayType`([getDayType()](../../com.aspose.tasks/weekday\#getDayType--)/[setDayType(int)](../../com.aspose.tasks/weekday\#setDayType-int-)) में कास्ट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| dw | int | कास्ट करने के लिए सप्ताह का दिन। |

**Returns:**
int - एक कास्ट किया हुआ दिन प्रकार।
### createDefaultWorkingDay(int dayType) {#createDefaultWorkingDay-int-}
```
public static WeekDay createDefaultWorkingDay(int dayType)
```


डिफ़ॉल्ट कार्य दिवस बनाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| dayType | int | डिफ़ॉल्ट कार्य दिवस बनाने के लिए दिन प्रकार। |

**Returns:**
[WeekDay](../../com.aspose.tasks/weekday) - A default working day with working times 8-12 and 13-17.
### deepClone() {#deepClone--}
```
public final WeekDay deepClone()
```


सप्ताह के दिन की गहरी कॉपी लौटाता है।

**Returns:**
[WeekDay](../../com.aspose.tasks/weekday) - Returns the deep copy of the week day.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| obj | java.lang.Object | इस इंस्टेंस की तुलना करने के लिए ऑब्जेक्ट। |

**Returns:**
boolean - **True** यदि निर्दिष्ट वस्तु एक WeekDay है जिसका FromDate, ToDate मान और WorkingTimes इस उदाहरण के समान हैं; अन्यथा, **false**.
### getDayType() {#getDayType--}
```
public final int getDayType()
```


एक दिन का प्रकार प्राप्त करता है।

**Returns:**
int - दिन का प्रकार।
### getDayWorking() {#getDayWorking--}
```
public final boolean getDayWorking()
```


एक मान प्राप्त करता है जो दर्शाता है कि निर्दिष्ट तिथि या दिन प्रकार कार्यशील है या नहीं।

**Returns:**
boolean - एक मान जो दर्शाता है कि निर्दिष्ट तिथि या दिन प्रकार कार्यशील है या नहीं।
### getFromDate() {#getFromDate--}
```
public final Date getFromDate()
```


एक अपवाद समय की शुरुआत प्राप्त करता है।

**Returns:**
java.util.Date - अपवाद समय की शुरुआत।
### getToDate() {#getToDate--}
```
public final Date getToDate()
```


एक अपवाद समय का अंत प्राप्त करता है।

**Returns:**
java.util.Date - अपवाद समय का अंत।
### getWorkingTime() {#getWorkingTime--}
```
public final double getWorkingTime()
```


सप्ताह के दिन के लिए कार्य समय लौटाता है।

**Returns:**
double - कार्य समय।
### getWorkingTimes() {#getWorkingTimes--}
```
public final WorkingTimeCollection getWorkingTimes()
```


इस WeekDay उदाहरण के लिए WorkingTimeCollection प्राप्त करता है। कार्य समयों का संग्रह जो सप्ताह के दिन पर काम किए गए समय को परिभाषित करता है।

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - WorkingTimeCollection for this WeekDay instance.
### hashCode() {#hashCode--}
```
public int hashCode()
```


[WeekDay](../../com.aspose.tasks/weekday) वर्ग के उदाहरण के लिए हैश कोड मान लौटाता है।

**Returns:**
int - इस ऑब्जेक्ट के लिए हैश कोड मान लौटाता है।
### setDayWorking(boolean value) {#setDayWorking-boolean-}
```
public final void setDayWorking(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि निर्दिष्ट तिथि या दिन प्रकार कार्यशील है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि निर्दिष्ट तिथि या दिन प्रकार कार्यशील है या नहीं। |

### setDefaultWorkingTime(WeekDay day) {#setDefaultWorkingTime-com.aspose.tasks.WeekDay-}
```
public static void setDefaultWorkingTime(WeekDay day)
```


निर्दिष्ट सप्ताह के दिन के लिए डिफ़ॉल्ट समय अवधि सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| day | [WeekDay](../../com.aspose.tasks/weekday) | डिफ़ॉल्ट कार्य दिवस सेट करने के लिए सप्ताह का दिन। |

### setFromDate(Date value) {#setFromDate-java.util.Date-}
```
public final void setFromDate(Date value)
```


एक अपवाद समय की शुरुआत सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.Date | अपवाद समय की शुरुआत। |

### setToDate(Date value) {#setToDate-java.util.Date-}
```
public final void setToDate(Date value)
```


एक अपवाद समय का अंत सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.Date | अपवाद समय का अंत। |

