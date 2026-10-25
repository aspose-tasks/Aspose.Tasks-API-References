---
title: "RiskPattern"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل نمط خطر لمهمة مشروع."
type: docs
weight: 268
url: /ar/java/com.aspose.tasks/riskpattern/
---

**Inheritance:**
java.lang.Object
```
public class RiskPattern
```

يمثل نمط خطر لمهمة مشروع.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [RiskPattern(Task task)](#RiskPattern-com.aspose.tasks.Task-) | ينشئ مثالا جديدا من الفئة [RiskPattern](../../com.aspose.tasks/riskpattern). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getConfidenceLevel()](#getConfidenceLevel--) | يحصل على مستوى الثقة الذي يتطابق مع نسبة الوقت التي تكون فيها القيم المولدة فعليًا ضمن التقديرات المتفائلة والمتشائمة. |
| [getDistribution()](#getDistribution--) | يحصل على توزيع الاحتمال المستخدم في محاكاة مونت كارلو. |
| [getOptimistic()](#getOptimistic--) | يحصل على النسبة المئوية للمدة الأكثر احتمالًا للمهمة والتي يمكن أن تحدث في أفضل سيناريو ممكن للمشروع. |
| [getPessimistic()](#getPessimistic--) | يحصل على النسبة المئوية للمدة الأكثر احتمالًا للمهمة والتي يمكن أن تحدث في أسوأ سيناريو ممكن للمشروع. |
| [getTask()](#getTask--) | يحصل على مهمة مشروع يتم تطبيق نمط المخاطر هذا عليها. |
| [setConfidenceLevel(int value)](#setConfidenceLevel-int-) | يضبط مستوى الثقة الذي يتطابق مع النسبة المئوية للوقت الذي ستكون فيه القيم المولدة الفعلية ضمن التقديرات المتفائلة والمتشائمة. |
| [setDistribution(int value)](#setDistribution-int-) | يضبط توزيع الاحتمال المستخدم في محاكاة مونت كارلو. |
| [setOptimistic(int value)](#setOptimistic-int-) | يضبط النسبة المئوية للمدة الأكثر احتمالًا للمهمة التي يمكن أن تحدث في أفضل سيناريو مشروع ممكن. |
| [setPessimistic(int value)](#setPessimistic-int-) | يضبط النسبة المئوية للمدة الأكثر احتمالًا للمهمة التي يمكن أن تحدث في أسوأ سيناريو مشروع ممكن. |
### RiskPattern(Task task) {#RiskPattern-com.aspose.tasks.Task-}
```
public RiskPattern(Task task)
```


ينشئ مثالا جديدا من الفئة [RiskPattern](../../com.aspose.tasks/riskpattern).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | المهمة المشروع المحددة التي سيُطبق عليها هذا الخطر في محاكاة مونت كارلو. |

### getConfidenceLevel() {#getConfidenceLevel--}
```
public final int getConfidenceLevel()
```


يحصل على مستوى الثقة الذي يتطابق مع النسبة المئوية للوقت الذي ستكون فيه القيم المولدة الفعلية ضمن التقديرات المتفائلة والمتشائمة. القيمة الافتراضية هي CL99.

--------------------

يمكن أن تكون واحدة من القيم المعرفة في تعداد `ConfidenceLevel`([getConfidenceLevel()](../../com.aspose/tasks/riskpattern\#getConfidenceLevel--)/[setConfidenceLevel(int)](../../com.aspose/tasks/riskpattern\#setConfidenceLevel-int-)).

**Returns:**
int - مستوى الثقة الذي يتطابق مع النسبة المئوية للوقت الذي ستكون فيه القيم المولدة الفعلية ضمن التقديرات المتفائلة والمتشائمة.
### getDistribution() {#getDistribution--}
```
public final int getDistribution()
```


يحصل على توزيع الاحتمال المستخدم في محاكاة مونت كارلو. القيمة الافتراضية هي ProbabilityDistributionType.Normal.

--------------------

يمكن أن تكون واحدة من القيم المعرفة في تعداد [ProbabilityDistributionType](../../com.aspose/tasks/probabilitydistributiontype).

**Returns:**
int - توزيع الاحتمال المستخدم في محاكاة مونت كارلو.
### getOptimistic() {#getOptimistic--}
```
public final int getOptimistic()
```


يحصل على النسبة المئوية للمدة الأكثر احتمالًا للمهمة التي يمكن أن تحدث في أفضل سيناريو مشروع ممكن. القيمة الافتراضية هي 75، مما يعني أنه إذا كانت المدة المقدرة للمهمة المحددة هي 4 أيام فإن المدة المتفائلة ستكون 3 أيام.

**Returns:**
int - النسبة المئوية للمدة الأكثر احتمالًا للمهمة التي يمكن أن تحدث في أفضل سيناريو مشروع ممكن.
### getPessimistic() {#getPessimistic--}
```
public final int getPessimistic()
```


يحصل على النسبة المئوية للمدة الأكثر احتمالًا للمهمة التي يمكن أن تحدث في أسوأ سيناريو مشروع ممكن. القيمة الافتراضية هي 125، مما يعني أنه إذا كانت المدة المقدرة للمهمة المحددة هي 4 أيام فإن المدة المتشائمة ستكون 5 أيام.

**Returns:**
int - النسبة المئوية للمدة الأكثر احتمالًا للمهمة التي يمكن أن تحدث في أسوأ سيناريو مشروع ممكن.
### getTask() {#getTask--}
```
public final Task getTask()
```


يحصل على مهمة مشروع يتم تطبيق نمط المخاطر هذا عليها.

**Returns:**
[Task](../../com.aspose.tasks/task) - a project task to which this risk pattern is applied.
### setConfidenceLevel(int value) {#setConfidenceLevel-int-}
```
public final void setConfidenceLevel(int value)
```


يضبط مستوى الثقة الذي يتطابق مع النسبة المئوية للوقت الذي ستكون فيه القيم المولدة الفعلية ضمن التقديرات المتفائلة والمتشائمة. القيمة الافتراضية هي CL99.

--------------------

يمكن أن تكون واحدة من القيم المعرفة في تعداد `ConfidenceLevel`([getConfidenceLevel()](../../com.aspose/tasks/riskpattern\#getConfidenceLevel--)/[setConfidenceLevel(int)](../../com.aspose/tasks/riskpattern\#setConfidenceLevel-int-)).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | مستوى الثقة الذي يتطابق مع النسبة المئوية للوقت الذي ستكون فيه القيم المولدة الفعلية ضمن التقديرات المتفائلة والمتشائمة. |

### setDistribution(int value) {#setDistribution-int-}
```
public final void setDistribution(int value)
```


يضبط توزيع الاحتمال المستخدم في محاكاة مونت كارلو. القيمة الافتراضية هي ProbabilityDistributionType.Normal.

--------------------

يمكن أن تكون واحدة من القيم المعرفة في تعداد [ProbabilityDistributionType](../../com.aspose/tasks/probabilitydistributiontype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | توزيع الاحتمال المستخدم في محاكاة مونت كارلو. |

### setOptimistic(int value) {#setOptimistic-int-}
```
public final void setOptimistic(int value)
```


يضبط النسبة المئوية للمدة الأكثر احتمالًا للمهمة التي يمكن أن تحدث في أفضل سيناريو مشروع ممكن. القيمة الافتراضية هي 75، مما يعني أنه إذا كانت المدة المقدرة للمهمة المحددة هي 4 أيام فإن المدة المتفائلة ستكون 3 أيام.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | النسبة المئوية للمدة الأكثر احتمالًا للمهمة التي يمكن أن تحدث في أفضل سيناريو مشروع ممكن. |

### setPessimistic(int value) {#setPessimistic-int-}
```
public final void setPessimistic(int value)
```


يضبط النسبة المئوية للمدة الأكثر احتمالًا للمهمة التي يمكن أن تحدث في أسوأ سيناريو مشروع ممكن. القيمة الافتراضية هي 125، مما يعني أنه إذا كانت المدة المقدرة للمهمة المحددة هي 4 أيام فإن المدة المتشائمة ستكون 5 أيام.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | النسبة المئوية للمدة الأكثر احتمالًا للمهمة التي يمكن أن تحدث في أسوأ سيناريو مشروع ممكن. |

