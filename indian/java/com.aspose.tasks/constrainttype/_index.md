---
title: "ConstraintType"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "कार्य की प्रारंभ या समाप्ति तिथि पर प्रतिबंध को निर्दिष्ट करता है।"
type: docs
weight: 52
url: /hi/java/com.aspose.tasks/constrainttype/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class ConstraintType extends System.Enum
```

एक कार्य की प्रारंभ या समाप्ति तिथि पर प्रतिबंध निर्दिष्ट करता है। XML में निर्यात करते समय Undefined मानों को परिणामी XML से हटा दिया जाएगा।
## फ़ील्ड्स

| फ़ील्ड | विवरण |
| --- | --- |
| [AsLateAsPossible](#AsLateAsPossible) | `Task` के `Tsk.Start` और `Tsk.Finish` तिथियों को पैरेंट `Tsk.Start` और `Tsk.Finish` तिथियों के सापेक्ष ALAP के रूप में निर्धारित किया गया है और `Project.TaskLinks` को ध्यान में रखते हुए। |
| [AsSoonAsPossible](#AsSoonAsPossible) | `Task` के `Tsk.Start` और `Tsk.Finish` तिथियों को पैरेंट `Tsk.Start` और `Tsk.Finish` तिथियों के सापेक्ष ASAP के रूप में निर्धारित किया गया है और `Project.TaskLinks` को ध्यान में रखते हुए। |
| [FinishNoEarlierThan](#FinishNoEarlierThan) | समाप्ति इससे पहले नहीं |
| [FinishNoLaterThan](#FinishNoLaterThan) | अंतिम तिथि इससे बाद नहीं |
| [MustFinishOn](#MustFinishOn) | समाप्त होना चाहिए |
| [MustStartOn](#MustStartOn) | प्रारम्भ होना चाहिए |
| [StartNoEarlierThan](#StartNoEarlierThan) | प्रारम्भ इससे पहले नहीं |
| [StartNoLaterThan](#StartNoLaterThan) | प्रारम्भ इससे बाद नहीं |
| [Undefined](#Undefined) | मूल प्रोजेक्ट फ़ाइल में मान परिभाषित नहीं था। |
### AsLateAsPossible {#AsLateAsPossible}
```
public static final int AsLateAsPossible
```


`Task` के `Tsk.Start` और `Tsk.Finish` तिथियों को पैरेंट `Tsk.Start` और `Tsk.Finish` तिथियों के सापेक्ष ALAP के रूप में निर्धारित किया गया है और `Project.TaskLinks` को ध्यान में रखते हुए।

### AsSoonAsPossible {#AsSoonAsPossible}
```
public static final int AsSoonAsPossible
```


`Task` के `Tsk.Start` और `Tsk.Finish` तिथियों को पैरेंट `Tsk.Start` और `Tsk.Finish` तिथियों के सापेक्ष ASAP के रूप में निर्धारित किया गया है और `Project.TaskLinks` को ध्यान में रखते हुए।

### FinishNoEarlierThan {#FinishNoEarlierThan}
```
public static final int FinishNoEarlierThan
```


समाप्ति इससे पहले नहीं

### FinishNoLaterThan {#FinishNoLaterThan}
```
public static final int FinishNoLaterThan
```


अंतिम तिथि इससे बाद नहीं

### MustFinishOn {#MustFinishOn}
```
public static final int MustFinishOn
```


समाप्त होना चाहिए

### MustStartOn {#MustStartOn}
```
public static final int MustStartOn
```


प्रारम्भ होना चाहिए

### StartNoEarlierThan {#StartNoEarlierThan}
```
public static final int StartNoEarlierThan
```


प्रारम्भ इससे पहले नहीं

### StartNoLaterThan {#StartNoLaterThan}
```
public static final int StartNoLaterThan
```


प्रारम्भ इससे बाद नहीं

### Undefined {#Undefined}
```
public static final int Undefined
```


मूल प्रोजेक्ट फ़ाइल में मान परिभाषित नहीं था।

