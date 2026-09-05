---
title: "DailyRepetitionBase"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "दैनिक आवृत्ति पैटर्न में पुनरावृत्तियों के लिए बेस क्लास का प्रतिनिधित्व करता है।"
type: docs
weight: 65
url: /hi/java/com.aspose.tasks/dailyrepetitionbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.IValidatorCreator, com.aspose.tasks.ICalculatorCreator
```
public abstract class DailyRepetitionBase implements IValidatorCreator, ICalculatorCreator
```

दैनिक आवृत्ति पैटर्न में पुनरावृत्तियों के लिए बेस क्लास का प्रतिनिधित्व करता है।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getCalculator(Calendar calendar, Duration duration)](#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-) | \{@inheritDoc\} |
| [getRepetitionInterval()](#getRepetitionInterval--) | एक संख्या प्राप्त करता है जो घटनाओं के बीच दिनों में अंतराल को दर्शाती है। |
| [getValidator(Calendar calendar)](#getValidator-com.aspose.tasks.Calendar-) | \{@inheritDoc\} |
| [setRepetitionInterval(int value)](#setRepetitionInterval-int-) | एक संख्या सेट करता है जो घटनाओं के बीच दिनों में अंतराल को दर्शाती है। |
### getCalculator(Calendar calendar, Duration duration) {#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-}
```
public final RecurrenceDateCalculatorBase getCalculator(Calendar calendar, Duration duration)
```


एक कैलकुलेटर प्राप्त करता है जिसका उपयोग पुनरावृत्ति की गणना के लिए किया जाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |
| duration | [Duration](../../com.aspose.tasks/duration) | \{@inheritDoc\} |

**Returns:**
com.aspose.tasks.RecurrenceDateCalculatorBase - \{@inheritDoc\}
### getRepetitionInterval() {#getRepetitionInterval--}
```
public final int getRepetitionInterval()
```


एक संख्या प्राप्त करता है जो घटनाओं के बीच दिनों में अंतराल को दर्शाती है।

**Returns:**
int - एक संख्या जो घटनाओं के बीच दिनों में अंतराल को दर्शाती है।
### getValidator(Calendar calendar) {#getValidator-com.aspose.tasks.Calendar-}
```
public final RecurrencePatternValidatorBase getValidator(Calendar calendar)
```


आवर्ती पैटर्न के लिए एक वैलिडेटर प्राप्त करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |

**Returns:**
com.aspose.tasks.RecurrencePatternValidatorBase - \{@inheritDoc\}
### setRepetitionInterval(int value) {#setRepetitionInterval-int-}
```
public final void setRepetitionInterval(int value)
```


एक संख्या सेट करता है जो घटनाओं के बीच दिनों में अंतराल को दर्शाती है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | एक संख्या जो घटनाओं के बीच दिनों में अंतराल को दर्शाती है। |

