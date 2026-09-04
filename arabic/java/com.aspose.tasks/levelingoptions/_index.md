---
title: "LevelingOptions"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يسمح بتحديد معلمات تسوية الموارد."
type: docs
weight: 142
url: /ar/java/com.aspose.tasks/levelingoptions/
---

**Inheritance:**
java.lang.Object
```
public final class LevelingOptions
```

يسمح بتحديد معلمات تسوية الموارد.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [LevelingOptions()](#LevelingOptions--) | ينشئ مثيلاً جديداً من الفئة [LevelingOptions](../../com.aspose/tasks/levelingoptions). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getCancellationToken()](#getCancellationToken--) | يحصل على رمز يمكن استخدامه لإلغاء عملية تسوية المشروع. |
| [getFinishDate()](#getFinishDate--) | يحصل على تاريخ انتهاء فترة التسوية. |
| [getLevelingOrder()](#getLevelingOrder--) | يحصل على الترتيب الذي تؤخر به خوارزمية التسوية المهام التي لديها تخصيص زائد. |
| [getMessageHandler()](#getMessageHandler--) | يحصل على رد نداء معالج الرسائل الذي يمكن استخدامه لاعتراض رسائل السجل التي ينتجها Aspose.Tasks أثناء تسوية الموارد. |
| [getMessageLevel()](#getMessageLevel--) | يحصل على مستوى رسائل السجل التي ينتجها Aspose.Tasks أثناء تسوية الموارد. |
| [getResources()](#getResources--) | يحصل على قائمة الموارد التي سيتم تسويتها. |
| [getStartDate()](#getStartDate--) | يحصل على تاريخ بدء فترة التسوية. |
| [setCancellationToken(CancellationToken value)](#setCancellationToken-com.aspose.tasks.CancellationToken-) | يضبط رمزًا يمكن استخدامه لإلغاء عملية تسوية المشروع. |
| [setFinishDate(Date value)](#setFinishDate-java.util.Date-) | يضبط تاريخ انتهاء فترة التسوية. |
| [setLevelingOrder(int value)](#setLevelingOrder-int-) | الترتيب الذي تؤخر فيه خوارزمية التسوية المهام التي لديها تخصيصات زائدة. |
| [setMessageHandler(IMessageHandler value)](#setMessageHandler-com.aspose.tasks.IMessageHandler-) | يضبط رد نداء معالج الرسائل الذي يمكن استخدامه لاعتراض رسائل السجل التي ينتجها **Aspose.Tasks** أثناء تسوية الموارد. |
| [setMessageLevel(int value)](#setMessageLevel-int-) | يضبط مستوى رسائل السجل التي ينتجها **Aspose.Tasks** أثناء تسوية الموارد. |
| [setResources(List&lt;Resource&gt; value)](#setResources-java.util.List-com.aspose.tasks.Resource--) | يضبط قائمة الموارد التي سيتم تسويتها. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | يضبط تاريخ بدء فترة التسوية. |
### LevelingOptions() {#LevelingOptions--}
```
public LevelingOptions()
```


ينشئ مثيلاً جديداً من الفئة [LevelingOptions](../../com.aspose/tasks/levelingoptions).

### getCancellationToken() {#getCancellationToken--}
```
public final CancellationToken getCancellationToken()
```


يحصل على رمز يمكن استخدامه لإلغاء عملية تسوية المشروع.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token which can be used to cancel a project leveling operation.
### getFinishDate() {#getFinishDate--}
```
public final Date getFinishDate()
```


يحصل على تاريخ انتهاء فترة التسوية. القيمة الافتراضية هي تاريخ انتهاء المشروع.

**Returns:**
java.util.Date - تاريخ انتهاء فترة التسوية.
### getLevelingOrder() {#getLevelingOrder--}
```
public final int getLevelingOrder()
```


يحصل على الترتيب الذي تؤخر فيه خوارزمية التسوية المهام التي لديها تخصيصات زائدة. بعد تحديد المهام التي تسبب التخصيص الزائد والمهام التي يمكن تأخيرها، يُستخدم الترتيب المحدد لتحديد أي مهمة يجب تأخيرها أولاً.

**Returns:**
int - الترتيب الذي تؤخر فيه خوارزمية التسوية المهام التي لديها تخصيصات زائدة.
### getMessageHandler() {#getMessageHandler--}
```
public final IMessageHandler getMessageHandler()
```


يحصل على رد نداء معالج الرسائل الذي يمكن استخدامه لاعتراض رسائل السجل التي ينتجها Aspose.Tasks أثناء تسوية الموارد.

**Returns:**
[IMessageHandler](../../com.aspose.tasks/imessagehandler) - message handler callback which can be used to intercept log messages produced by Aspose.
### getMessageLevel() {#getMessageLevel--}
```
public final int getMessageLevel()
```


يحصل على مستوى رسائل السجل التي ينتجها Aspose.Tasks أثناء تسوية الموارد.

**Returns:**
int - مستوى رسائل السجل التي ينتجها **Aspose**.
### getResources() {#getResources--}
```
public final List<Resource> getResources()
```


يحصل على قائمة الموارد التي سيتم تسويتها. إذا تم تعيين null، سيتم تسوية جميع موارد المشروع.

**Returns:**
java.util.List&lt;com.aspose.tasks.Resource&gt; - قائمة الموارد التي سيتم تسويتها.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


يحصل على تاريخ بدء فترة التسوية. القيمة الافتراضية هي تاريخ بدء المشروع.

**Returns:**
java.util.Date - تاريخ بدء فترة التسوية.
### setCancellationToken(CancellationToken value) {#setCancellationToken-com.aspose.tasks.CancellationToken-}
```
public final void setCancellationToken(CancellationToken value)
```


يضبط رمزًا يمكن استخدامه لإلغاء عملية تسوية المشروع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [CancellationToken](../../com.aspose.tasks/cancellationtoken) | رمز يمكن استخدامه لإلغاء عملية تسوية المشروع. |

### setFinishDate(Date value) {#setFinishDate-java.util.Date-}
```
public final void setFinishDate(Date value)
```


يضبط تاريخ انتهاء فترة التسوية. القيمة الافتراضية هي تاريخ انتهاء المشروع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | تاريخ انتهاء فترة التسوية. |

### setLevelingOrder(int value) {#setLevelingOrder-int-}
```
public final void setLevelingOrder(int value)
```


الترتيب الذي تؤخر فيه خوارزمية التسوية المهام التي لديها تخصيصات زائدة. بعد تحديد المهام التي تسبب التخصيص الزائد والمهام التي يمكن تأخيرها، يُستخدم الترتيب المحدد لتحديد أي مهمة يجب تأخيرها أولاً.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | الترتيب الذي تؤخر فيه خوارزمية التسوية المهام التي لديها تخصيصات زائدة. |

### setMessageHandler(IMessageHandler value) {#setMessageHandler-com.aspose.tasks.IMessageHandler-}
```
public final void setMessageHandler(IMessageHandler value)
```


يضبط رد نداء معالج الرسائل الذي يمكن استخدامه لاعتراض رسائل السجل التي ينتجها **Aspose.Tasks** أثناء تسوية الموارد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [IMessageHandler](../../com.aspose.tasks/imessagehandler) | رد نداء معالج الرسائل الذي يمكن استخدامه لاعتراض رسائل السجل التي ينتجها **Aspose**. |

### setMessageLevel(int value) {#setMessageLevel-int-}
```
public final void setMessageLevel(int value)
```


يضبط مستوى رسائل السجل التي ينتجها **Aspose.Tasks** أثناء تسوية الموارد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | مستوى رسائل السجل التي ينتجها **Aspose**. |

### setResources(List&lt;Resource&gt; value) {#setResources-java.util.List-com.aspose.tasks.Resource--}
```
public final void setResources(List<Resource> value)
```


يضبط قائمة الموارد التي سيتم تسويتها. إذا تم تعيين null، سيتم تسوية جميع موارد المشروع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.List&lt;com.aspose.tasks.Resource&gt; | قائمة الموارد التي سيتم تسويتها. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


يضبط تاريخ بدء فترة التسوية. القيمة الافتراضية هي تاريخ بدء المشروع`s.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | تاريخ بدء فترة التسوية. |

