---
title: "ByYearWeekDayRepetition"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "एक पैटर्न का प्रतिनिधित्व करता है जो महीने में सप्ताह के दिन की स्थिति पर आधारित है।"
type: docs
weight: 38
url: /hi/java/com.aspose.tasks/byyearweekdayrepetition/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.YearlyRepetitionBase](../../com.aspose.tasks/yearlyrepetitionbase)
```
public class ByYearWeekDayRepetition extends YearlyRepetitionBase
```

एक पैटर्न का प्रतिनिधित्व करता है जो महीने में सप्ताह के दिन की स्थिति पर आधारित है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [ByYearWeekDayRepetition()](#ByYearWeekDayRepetition--) | [ByYearWeekDayRepetition](../../com.aspose.tasks/byyearweekdayrepetition) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getMonth()](#getMonth--) | कार्य के दोहराए जाने वाले महीने को प्राप्त करता है। |
| [getPosition()](#getPosition--) | कार्य के दोहराए जाने वाले महीने के सप्ताह में दिन की स्थिति को प्राप्त करता है। |
| [getWeekDay()](#getWeekDay--) | कार्य के दोहराए जाने वाले सप्ताह के दिन के प्रकार को प्राप्त करता है। |
| [setMonth(int value)](#setMonth-int-) | कार्य के दोहराए जाने वाले महीने को सेट करता है। |
| [setPosition(int value)](#setPosition-int-) | कार्य के दोहराए जाने वाले महीने के सप्ताह में दिन की स्थिति को सेट करता है। |
| [setWeekDay(int value)](#setWeekDay-int-) | कार्य के दोहराए जाने वाले सप्ताह के दिन के प्रकार को सेट करता है। |
### ByYearWeekDayRepetition() {#ByYearWeekDayRepetition--}
```
public ByYearWeekDayRepetition()
```


[ByYearWeekDayRepetition](../../com.aspose.tasks/byyearweekdayrepetition) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

### getMonth() {#getMonth--}
```
public final int getMonth()
```


कार्य के दोहराए जाने वाले महीने को प्राप्त करता है।

`Month` को पढ़ें/लिखें।

**Returns:**
int - वह महीना जिसमें कार्य दोहराया जाना चाहिए।
### getPosition() {#getPosition--}
```
public final int getPosition()
```


कार्य के दोहराए जाने वाले महीने के सप्ताह में दिन की स्थिति को प्राप्त करता है।

पढ़ें/लिखें `OrdinalNumber`.

**Returns:**
int - वह स्थिति जिसमें दिन सप्ताह के एक महीने में होता है, जिस पर कार्य को दोहराया जाना चाहिए।
### getWeekDay() {#getWeekDay--}
```
public final int getWeekDay()
```


कार्य के दोहराए जाने वाले सप्ताह के दिन के प्रकार को प्राप्त करता है।

पढ़ें/लिखें `DayOfWeek`.

**Returns:**
int - वह प्रकार का सप्ताह का दिन जिस पर कार्य को दोहराया जाना चाहिए।
### setMonth(int value) {#setMonth-int-}
```
public final void setMonth(int value)
```


कार्य के दोहराए जाने वाले महीने को सेट करता है।

`Month` को पढ़ें/लिखें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | एक महीना जिस पर कार्य को दोहराया जाना चाहिए। |

### setPosition(int value) {#setPosition-int-}
```
public final void setPosition(int value)
```


कार्य के दोहराए जाने वाले महीने के सप्ताह में दिन की स्थिति को सेट करता है।

पढ़ें/लिखें `OrdinalNumber`.

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | एक स्थिति जिसमें दिन एक महीने के एक सप्ताह में होता है, जिस पर कार्य को दोहराया जाना चाहिए। |

### setWeekDay(int value) {#setWeekDay-int-}
```
public final void setWeekDay(int value)
```


कार्य के दोहराए जाने वाले सप्ताह के दिन के प्रकार को सेट करता है।

पढ़ें/लिखें `DayOfWeek`.

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | एक प्रकार का सप्ताह का दिन जिस पर कार्य को दोहराया जाना चाहिए। |

