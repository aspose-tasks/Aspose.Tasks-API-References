---
title: "RecurringTaskInfo"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "प्रोजेक्ट में एक आवर्ती कार्य के विवरण का प्रतिनिधित्व करता है।"
type: docs
weight: 244
url: /hi/java/com.aspose.tasks/recurringtaskinfo/
---

**Inheritance:**
java.lang.Object
```
public class RecurringTaskInfo
```

प्रोजेक्ट में एक आवर्ती कार्य के विवरण का प्रतिनिधित्व करता है।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getDailyRepetitions()](#getDailyRepetitions--) | दैनिक आवृत्ति पैटर्न के लिए दोहराव की संख्या प्राप्त करता है। |
| [getDailyUseWorkdays()](#getDailyUseWorkdays--) | दैनिक आवृत्ति पैटर्न के लिए कार्यदिवसों का उपयोग करना है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [getDuration()](#getDuration--) | आवर्ती कार्य की एक घटना की अवधि प्राप्त करता है। |
| [getEndDate()](#getEndDate--) | घटनाओं के समाप्त होने की तिथि प्राप्त करता है। |
| [getMonthlyDay()](#getMonthlyDay--) | मासिक आवृत्ति पैटर्न के दिन की संख्या प्राप्त करता है। |
| [getMonthlyOrdinalDay()](#getMonthlyOrdinalDay--) | क्रमांकित दिन का उपयोग करते समय मासिक आवृत्ति पैटर्न का दिन प्राप्त करता है। |
| [getMonthlyOrdinalNumber()](#getMonthlyOrdinalNumber--) | मासिक आवृत्ति पैटर्न का क्रमांकित संख्या प्राप्त करता है। |
| [getMonthlyOrdinalRepetitions()](#getMonthlyOrdinalRepetitions--) | क्रमांकित दिन का उपयोग करते समय मासिक आवृत्ति पैटर्न के दोहराव की संख्या प्राप्त करता है। |
| [getMonthlyRepetitions()](#getMonthlyRepetitions--) | मासिक आवृत्ति पैटर्न के दोहराव की संख्या प्राप्त करता है। |
| [getMonthlyUseOrdinalDay()](#getMonthlyUseOrdinalDay--) | मासिक आवृत्ति पैटर्न के लिए क्रमांकित दिन का उपयोग करना है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [getOccurrences()](#getOccurrences--) | आवर्ती कार्य की घटनाओं की संख्या प्राप्त करता है। |
| [getRecurrencePattern()](#getRecurrencePattern--) | आवर्ती कार्य का आवृत्ति पैटर्न प्राप्त करता है। |
| [getStartDate()](#getStartDate--) | घटनाओं के शुरू होने की तिथि प्राप्त करता है। |
| [getTask()](#getTask--) | इस [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) क्लास के उदाहरण का पैरेंट कार्य प्राप्त करता है। |
| [getUseEndDate()](#getUseEndDate--) | आवर्ती कार्य के लिए समाप्ति तिथि या घटनाओं की संख्या का उपयोग करना है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [getWeeklyDays()](#getWeeklyDays--) | साप्ताहिक आवृत्ति पैटर्न में उपयोग किए गए दिनों का संग्रह प्राप्त करता है। |
| [getWeeklyRepetitions()](#getWeeklyRepetitions--) | साप्ताहिक आवृत्ति पैटर्न के दोहराव की संख्या प्राप्त करता है। |
| [getYearlyDate()](#getYearlyDate--) | वार्षिक आवृत्ति पैटर्न की तिथि प्राप्त करता है। |
| [getYearlyOrdinalDay()](#getYearlyOrdinalDay--) | क्रमांकित दिन का उपयोग करते समय वार्षिक पुनरावृत्ति पैटर्न का एक सप्ताह का दिन प्राप्त करता है। |
| [getYearlyOrdinalMonth()](#getYearlyOrdinalMonth--) | क्रमांकित दिन का उपयोग करते समय वार्षिक पुनरावृत्ति पैटर्न का एक महीना प्राप्त करता है। |
| [getYearlyOrdinalNumber()](#getYearlyOrdinalNumber--) | वार्षिक पुनरावृत्ति पैटर्न का क्रमांकित संख्या प्राप्त करता है। |
| [getYearlyUseOrdinalDay()](#getYearlyUseOrdinalDay--) | वार्षिक पुनरावृत्ति पैटर्न के लिए क्रमांकित दिन का उपयोग करना है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [setDailyRepetitions(int value)](#setDailyRepetitions-int-) | दैनिक पुनरावृत्ति पैटर्न के लिए दोहराव की संख्या निर्धारित करता है। |
| [setDailyUseWorkdays(boolean value)](#setDailyUseWorkdays-boolean-) | दैनिक पुनरावृत्ति पैटर्न के लिए कार्यदिवसों का उपयोग करना है या नहीं, यह दर्शाने वाला मान निर्धारित करता है। |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | पुनरावर्ती कार्य की एक घटना की अवधि निर्धारित करता है। |
| [setEndDate(Date value)](#setEndDate-java.util.Date-) | घटनाओं के समाप्त होने की तिथि निर्धारित करता है। |
| [setMonthlyDay(int value)](#setMonthlyDay-int-) | मासिक पुनरावृत्ति पैटर्न के दिन की संख्या निर्धारित करता है। |
| [setMonthlyOrdinalDay(int value)](#setMonthlyOrdinalDay-int-) | क्रमांकित दिन का उपयोग करते समय मासिक पुनरावृत्ति पैटर्न का दिन निर्धारित करता है। |
| [setMonthlyOrdinalNumber(int value)](#setMonthlyOrdinalNumber-int-) | मासिक पुनरावृत्ति पैटर्न की क्रमांकित संख्या निर्धारित करता है। |
| [setMonthlyOrdinalRepetitions(int value)](#setMonthlyOrdinalRepetitions-int-) | क्रमांकित दिन का उपयोग करते समय मासिक पुनरावृत्ति पैटर्न के दोहराव की संख्या निर्धारित करता है। |
| [setMonthlyRepetitions(int value)](#setMonthlyRepetitions-int-) | मासिक पुनरावृत्ति पैटर्न के दोहराव की संख्या निर्धारित करता है। |
| [setMonthlyUseOrdinalDay(boolean value)](#setMonthlyUseOrdinalDay-boolean-) | मासिक पुनरावृत्ति पैटर्न के लिए क्रमांकित दिन का उपयोग करना है या नहीं, यह दर्शाने वाला मान निर्धारित करता है। |
| [setOccurrences(int value)](#setOccurrences-int-) | पुनरावर्ती कार्य की घटनाओं की संख्या निर्धारित करता है। |
| [setRecurrencePattern(int value)](#setRecurrencePattern-int-) | पुनरावर्ती कार्य का पुनरावृत्ति पैटर्न निर्धारित करता है। |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | घटनाओं के शुरू होने की तिथि निर्धारित करता है। |
| [setUseEndDate(boolean value)](#setUseEndDate-boolean-) | पुनरावर्ती कार्य के लिए समाप्ति तिथि या घटनाओं की संख्या का उपयोग करना है या नहीं, यह दर्शाने वाला मान निर्धारित करता है। |
| [setWeeklyDays(int value)](#setWeeklyDays-int-) | साप्ताहिक पुनरावृत्ति पैटर्न में उपयोग किए जाने वाले दिनों का संग्रह निर्धारित करता है। |
| [setWeeklyRepetitions(int value)](#setWeeklyRepetitions-int-) | साप्ताहिक पुनरावृत्ति पैटर्न के दोहराव की संख्या निर्धारित करता है। |
| [setYearlyDate(Date value)](#setYearlyDate-java.util.Date-) | वार्षिक पुनरावृत्ति पैटर्न की तिथि निर्धारित करता है। |
| [setYearlyOrdinalDay(int value)](#setYearlyOrdinalDay-int-) | क्रमांकित दिन का उपयोग करते समय वार्षिक पुनरावृत्ति पैटर्न का सप्ताह का दिन निर्धारित करता है। |
| [setYearlyOrdinalMonth(int value)](#setYearlyOrdinalMonth-int-) | क्रमांकित दिन का उपयोग करते समय वार्षिक पुनरावृत्ति पैटर्न का महीना निर्धारित करता है। |
| [setYearlyOrdinalNumber(int value)](#setYearlyOrdinalNumber-int-) | वार्षिक पुनरावृत्ति पैटर्न की क्रमांकित संख्या निर्धारित करता है। |
| [setYearlyUseOrdinalDay(boolean value)](#setYearlyUseOrdinalDay-boolean-) | वार्षिक पुनरावृत्ति पैटर्न के लिए क्रमांकित दिन का उपयोग करना है या नहीं, यह दर्शाने वाला मान निर्धारित करता है। |
### getDailyRepetitions() {#getDailyRepetitions--}
```
public final int getDailyRepetitions()
```


दैनिक आवृत्ति पैटर्न के लिए दोहराव की संख्या प्राप्त करता है।

**Returns:**
int - दैनिक आवृत्ति पैटर्न के लिए दोहराव की संख्या।
### getDailyUseWorkdays() {#getDailyUseWorkdays--}
```
public final boolean getDailyUseWorkdays()
```


दैनिक आवृत्ति पैटर्न के लिए कार्यदिवसों का उपयोग करना है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
boolean - एक मान जो दर्शाता है कि दैनिक आवृत्ति पैटर्न के लिए कार्यदिवसों का उपयोग किया जाए या नहीं।
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


आवर्ती कार्य की एक घटना की अवधि प्राप्त करता है।

--------------------

`Duration`([getDuration()](../../com.aspose.tasks/recurringtaskinfo\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskinfo\#setDuration-Duration-)) वर्ग का उदाहरण।

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the duration for one occurrence of the recurring task.
### getEndDate() {#getEndDate--}
```
public final Date getEndDate()
```


घटनाओं के समाप्त होने की तिथि प्राप्त करता है।

**Returns:**
java.util.Date - घटनाओं के समाप्त होने की तिथि।
### getMonthlyDay() {#getMonthlyDay--}
```
public final int getMonthlyDay()
```


मासिक आवृत्ति पैटर्न के दिन की संख्या प्राप्त करता है।

**Returns:**
int - मासिक आवृत्ति पैटर्न के दिन की संख्या।
### getMonthlyOrdinalDay() {#getMonthlyOrdinalDay--}
```
public final int getMonthlyOrdinalDay()
```


क्रमांकित दिन का उपयोग करते समय मासिक आवृत्ति पैटर्न का दिन प्राप्त करता है।

--------------------

[DayOfWeek](../../com.aspose.tasks/dayofweek) enumeration के मानों में से एक हो सकता है।

**Returns:**
int - क्रमांकित दिन का उपयोग करते समय मासिक आवृत्ति पैटर्न का दिन।
### getMonthlyOrdinalNumber() {#getMonthlyOrdinalNumber--}
```
public final int getMonthlyOrdinalNumber()
```


मासिक आवृत्ति पैटर्न का क्रमांकित संख्या प्राप्त करता है।

--------------------

[OrdinalNumber](../../com.aspose.tasks/ordinalnumber) enumeration के मानों में से एक हो सकता है।

**Returns:**
int - मासिक आवृत्ति पैटर्न का क्रमांकित संख्या।
### getMonthlyOrdinalRepetitions() {#getMonthlyOrdinalRepetitions--}
```
public final int getMonthlyOrdinalRepetitions()
```


क्रमांकित दिन का उपयोग करते समय मासिक आवृत्ति पैटर्न के दोहराव की संख्या प्राप्त करता है।

**Returns:**
int - क्रमांकित दिन का उपयोग करते समय मासिक आवृत्ति पैटर्न के दोहराव की संख्या।
### getMonthlyRepetitions() {#getMonthlyRepetitions--}
```
public final int getMonthlyRepetitions()
```


मासिक आवृत्ति पैटर्न के दोहराव की संख्या प्राप्त करता है।

**Returns:**
int - मासिक आवृत्ति पैटर्न के दोहराव की संख्या।
### getMonthlyUseOrdinalDay() {#getMonthlyUseOrdinalDay--}
```
public final boolean getMonthlyUseOrdinalDay()
```


मासिक आवृत्ति पैटर्न के लिए क्रमांकित दिन का उपयोग करना है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
boolean - एक मान जो दर्शाता है कि मासिक आवृत्ति पैटर्न के लिए क्रमांकित दिन का उपयोग किया जाए या नहीं।
### getOccurrences() {#getOccurrences--}
```
public final int getOccurrences()
```


आवर्ती कार्य की घटनाओं की संख्या प्राप्त करता है।

**Returns:**
int - आवर्ती कार्य की घटनाओं की संख्या।
### getRecurrencePattern() {#getRecurrencePattern--}
```
public final int getRecurrencePattern()
```


आवर्ती कार्य का आवृत्ति पैटर्न प्राप्त करता है।

--------------------

`RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskinfo\#getRecurrencePattern--)/[setRecurrencePattern(int)](../../com.aspose.tasks/recurringtaskinfo\#setRecurrencePattern-int-)) enumeration के मानों में से एक हो सकता है।

**Returns:**
int - आवर्ती कार्य का आवृत्ति पैटर्न।
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


घटनाओं के शुरू होने की तिथि प्राप्त करता है।

**Returns:**
java.util.Date - घटनाओं के शुरू होने की तिथि।
### getTask() {#getTask--}
```
public final Task getTask()
```


इस [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) क्लास के उदाहरण का पैरेंट कार्य प्राप्त करता है।

**Returns:**
[Task](../../com.aspose.tasks/task) - the parent task of this instance of [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) class.
### getUseEndDate() {#getUseEndDate--}
```
public final boolean getUseEndDate()
```


आवर्ती कार्य के लिए समाप्ति तिथि या घटनाओं की संख्या का उपयोग करना है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
boolean - एक मान जो दर्शाता है कि आवर्ती कार्य के लिए समाप्ति तिथि का उपयोग किया जाए या घटनाओं की संख्या।
### getWeeklyDays() {#getWeeklyDays--}
```
public final int getWeeklyDays()
```


साप्ताहिक आवृत्ति पैटर्न में उपयोग किए गए दिनों का संग्रह प्राप्त करता है।

--------------------

**Returns:**
int - साप्ताहिक आवृत्ति पैटर्न में उपयोग किए जाने वाले दिनों का संग्रह।
### getWeeklyRepetitions() {#getWeeklyRepetitions--}
```
public final int getWeeklyRepetitions()
```


साप्ताहिक आवृत्ति पैटर्न के दोहराव की संख्या प्राप्त करता है।

**Returns:**
int - साप्ताहिक आवृत्ति पैटर्न के दोहराव की संख्या।
### getYearlyDate() {#getYearlyDate--}
```
public final Date getYearlyDate()
```


वार्षिक आवृत्ति पैटर्न की तिथि प्राप्त करता है।

**Returns:**
java.util.Date - वार्षिक आवृत्ति पैटर्न की तिथि।
### getYearlyOrdinalDay() {#getYearlyOrdinalDay--}
```
public final int getYearlyOrdinalDay()
```


क्रमांकित दिन का उपयोग करते समय वार्षिक पुनरावृत्ति पैटर्न का एक सप्ताह का दिन प्राप्त करता है।

--------------------

[DayOfWeek](../../com.aspose.tasks/dayofweek) enumeration के मानों में से एक हो सकता है।

**Returns:**
int - क्रमांकित दिन का उपयोग करते समय वार्षिक आवृत्ति पैटर्न का सप्ताह का दिन।
### getYearlyOrdinalMonth() {#getYearlyOrdinalMonth--}
```
public final int getYearlyOrdinalMonth()
```


क्रमांकित दिन का उपयोग करते समय वार्षिक पुनरावृत्ति पैटर्न का एक महीना प्राप्त करता है।

--------------------

[Month](../../com.aspose.tasks/month) enumeration के मानों में से एक हो सकता है।

**Returns:**
int - क्रमांकित दिन का उपयोग करते समय वार्षिक आवृत्ति पैटर्न का महीना।
### getYearlyOrdinalNumber() {#getYearlyOrdinalNumber--}
```
public final int getYearlyOrdinalNumber()
```


वार्षिक पुनरावृत्ति पैटर्न का क्रमांकित संख्या प्राप्त करता है।

--------------------

[OrdinalNumber](../../com.aspose.tasks/ordinalnumber) enumeration के मानों में से एक हो सकता है।

**Returns:**
int - वार्षिक आवृत्ति पैटर्न का क्रमांकित संख्या।
### getYearlyUseOrdinalDay() {#getYearlyUseOrdinalDay--}
```
public final boolean getYearlyUseOrdinalDay()
```


वार्षिक पुनरावृत्ति पैटर्न के लिए क्रमांकित दिन का उपयोग करना है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
boolean - एक मान जो दर्शाता है कि वार्षिक आवृत्ति पैटर्न के लिए क्रमांकित दिन का उपयोग किया जाए या नहीं।
### setDailyRepetitions(int value) {#setDailyRepetitions-int-}
```
public final void setDailyRepetitions(int value)
```


दैनिक पुनरावृत्ति पैटर्न के लिए दोहराव की संख्या निर्धारित करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | दैनिक पुनरावृत्ति पैटर्न के लिए दोहराव की संख्या। |

### setDailyUseWorkdays(boolean value) {#setDailyUseWorkdays-boolean-}
```
public final void setDailyUseWorkdays(boolean value)
```


दैनिक पुनरावृत्ति पैटर्न के लिए कार्यदिवसों का उपयोग करना है या नहीं, यह दर्शाने वाला मान निर्धारित करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि दैनिक पुनरावृत्ति पैटर्न के लिए कार्यदिवसों का उपयोग किया जाए या नहीं। |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


पुनरावर्ती कार्य की एक घटना की अवधि निर्धारित करता है।

--------------------

`Duration`([getDuration()](../../com.aspose.tasks/recurringtaskinfo\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskinfo\#setDuration-Duration-)) वर्ग का उदाहरण।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | पुनरावर्ती कार्य की एक घटना की अवधि। |

### setEndDate(Date value) {#setEndDate-java.util.Date-}
```
public final void setEndDate(Date value)
```


घटनाओं के समाप्त होने की तिथि निर्धारित करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.Date | घटनाओं के समाप्त होने की तिथि। |

### setMonthlyDay(int value) {#setMonthlyDay-int-}
```
public final void setMonthlyDay(int value)
```


मासिक पुनरावृत्ति पैटर्न के दिन की संख्या निर्धारित करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | मासिक पुनरावृत्ति पैटर्न के दिन की संख्या। |

### setMonthlyOrdinalDay(int value) {#setMonthlyOrdinalDay-int-}
```
public final void setMonthlyOrdinalDay(int value)
```


क्रमांकित दिन का उपयोग करते समय मासिक पुनरावृत्ति पैटर्न का दिन निर्धारित करता है।

--------------------

[DayOfWeek](../../com.aspose.tasks/dayofweek) enumeration के मानों में से एक हो सकता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | क्रमांकित दिन का उपयोग करते समय मासिक पुनरावृत्ति पैटर्न का एक दिन। |

### setMonthlyOrdinalNumber(int value) {#setMonthlyOrdinalNumber-int-}
```
public final void setMonthlyOrdinalNumber(int value)
```


मासिक पुनरावृत्ति पैटर्न की क्रमांकित संख्या निर्धारित करता है।

--------------------

[OrdinalNumber](../../com.aspose.tasks/ordinalnumber) enumeration के मानों में से एक हो सकता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | मासिक पुनरावृत्ति पैटर्न का क्रमांकित संख्या। |

### setMonthlyOrdinalRepetitions(int value) {#setMonthlyOrdinalRepetitions-int-}
```
public final void setMonthlyOrdinalRepetitions(int value)
```


क्रमांकित दिन का उपयोग करते समय मासिक पुनरावृत्ति पैटर्न के दोहराव की संख्या निर्धारित करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | क्रमांकित दिन का उपयोग करते समय मासिक पुनरावृत्ति पैटर्न के दोहराव की संख्या। |

### setMonthlyRepetitions(int value) {#setMonthlyRepetitions-int-}
```
public final void setMonthlyRepetitions(int value)
```


मासिक पुनरावृत्ति पैटर्न के दोहराव की संख्या निर्धारित करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | मासिक पुनरावृत्ति पैटर्न के दोहराव की संख्या। |

### setMonthlyUseOrdinalDay(boolean value) {#setMonthlyUseOrdinalDay-boolean-}
```
public final void setMonthlyUseOrdinalDay(boolean value)
```


मासिक पुनरावृत्ति पैटर्न के लिए क्रमांकित दिन का उपयोग करना है या नहीं, यह दर्शाने वाला मान निर्धारित करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि मासिक पुनरावृत्ति पैटर्न के लिए क्रमांकित दिन का उपयोग किया जाए या नहीं। |

### setOccurrences(int value) {#setOccurrences-int-}
```
public final void setOccurrences(int value)
```


पुनरावर्ती कार्य की घटनाओं की संख्या निर्धारित करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | पुनरावर्ती कार्य की घटनाओं की संख्या। |

### setRecurrencePattern(int value) {#setRecurrencePattern-int-}
```
public final void setRecurrencePattern(int value)
```


पुनरावर्ती कार्य का पुनरावृत्ति पैटर्न निर्धारित करता है।

--------------------

`RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskinfo\#getRecurrencePattern--)/[setRecurrencePattern(int)](../../com.aspose.tasks/recurringtaskinfo\#setRecurrencePattern-int-)) enumeration के मानों में से एक हो सकता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | पुनरावर्ती कार्य का पुनरावृत्ति पैटर्न। |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


घटनाओं के शुरू होने की तिथि निर्धारित करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.Date | घटनाओं के शुरू होने की तिथि। |

### setUseEndDate(boolean value) {#setUseEndDate-boolean-}
```
public final void setUseEndDate(boolean value)
```


पुनरावर्ती कार्य के लिए समाप्ति तिथि या घटनाओं की संख्या का उपयोग करना है या नहीं, यह दर्शाने वाला मान निर्धारित करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि पुनरावर्ती कार्य के लिए समाप्ति तिथि या घटनाओं की संख्या का उपयोग किया जाए। |

### setWeeklyDays(int value) {#setWeeklyDays-int-}
```
public final void setWeeklyDays(int value)
```


साप्ताहिक पुनरावृत्ति पैटर्न में उपयोग किए जाने वाले दिनों का संग्रह निर्धारित करता है।

--------------------

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | साप्ताहिक पुनरावृत्ति पैटर्न में उपयोग किए जाने वाले दिनों का संग्रह। |

### setWeeklyRepetitions(int value) {#setWeeklyRepetitions-int-}
```
public final void setWeeklyRepetitions(int value)
```


साप्ताहिक पुनरावृत्ति पैटर्न के दोहराव की संख्या निर्धारित करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | साप्ताहिक पुनरावृत्ति पैटर्न के दोहराव की संख्या। |

### setYearlyDate(Date value) {#setYearlyDate-java.util.Date-}
```
public final void setYearlyDate(Date value)
```


वार्षिक पुनरावृत्ति पैटर्न की तिथि निर्धारित करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.Date | वार्षिक पुनरावृत्ति पैटर्न की तिथि। |

### setYearlyOrdinalDay(int value) {#setYearlyOrdinalDay-int-}
```
public final void setYearlyOrdinalDay(int value)
```


क्रमांकित दिन का उपयोग करते समय वार्षिक पुनरावृत्ति पैटर्न का सप्ताह का दिन निर्धारित करता है।

--------------------

[DayOfWeek](../../com.aspose.tasks/dayofweek) enumeration के मानों में से एक हो सकता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | क्रमांकित दिन का उपयोग करते समय वार्षिक पुनरावृत्ति पैटर्न का एक सप्ताह का दिन। |

### setYearlyOrdinalMonth(int value) {#setYearlyOrdinalMonth-int-}
```
public final void setYearlyOrdinalMonth(int value)
```


क्रमांकित दिन का उपयोग करते समय वार्षिक पुनरावृत्ति पैटर्न का महीना निर्धारित करता है।

--------------------

[Month](../../com.aspose.tasks/month) enumeration के मानों में से एक हो सकता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | क्रमांकित दिन का उपयोग करते समय वार्षिक पुनरावृत्ति पैटर्न का एक महीना। |

### setYearlyOrdinalNumber(int value) {#setYearlyOrdinalNumber-int-}
```
public final void setYearlyOrdinalNumber(int value)
```


वार्षिक पुनरावृत्ति पैटर्न की क्रमांकित संख्या निर्धारित करता है।

--------------------

[OrdinalNumber](../../com.aspose.tasks/ordinalnumber) enumeration के मानों में से एक हो सकता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | वार्षिक पुनरावृत्ति पैटर्न का क्रमांकित संख्या। |

### setYearlyUseOrdinalDay(boolean value) {#setYearlyUseOrdinalDay-boolean-}
```
public final void setYearlyUseOrdinalDay(boolean value)
```


वार्षिक पुनरावृत्ति पैटर्न के लिए क्रमांकित दिन का उपयोग करना है या नहीं, यह दर्शाने वाला मान निर्धारित करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि वार्षिक पुनरावृत्ति पैटर्न के लिए क्रमांकित दिन का उपयोग किया जाए या नहीं। |

