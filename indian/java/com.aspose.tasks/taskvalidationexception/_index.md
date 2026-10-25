---
title: "TaskValidationException"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "एक अपवाद को दर्शाता है जो पुनर्गणना के बाद प्रोजेक्ट कार्यों में त्रुटियों के मिलने पर फेंका जाता है।"
type: docs
weight: 308
url: /hi/java/com.aspose.tasks/taskvalidationexception/
---

**Inheritance:**
java.lang.Object, java.lang.Throwable, java.lang.Exception, java.lang.RuntimeException, com.aspose.ms.System.Exception, com.aspose.ms.System.ApplicationException, [com.aspose.tasks.ValidationException](../../com.aspose.tasks/validationexception), [com.aspose.tasks.RecalculationValidationException](../../com.aspose.tasks/recalculationvalidationexception)
```
public class TaskValidationException extends RecalculationValidationException
```

पुनर्गणना के बाद प्रोजेक्ट के टास्क में त्रुटियों के मिलने पर फेंकी जाने वाली अपवाद का प्रतिनिधित्व करता है।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getTask()](#getTask--) | उस कार्य को प्राप्त करता है जिसने अपवाद उत्पन्न किया। |
### getTask() {#getTask--}
```
public final Task getTask()
```


उस कार्य को प्राप्त करता है जिसने अपवाद उत्पन्न किया।

**Returns:**
[Task](../../com.aspose.tasks/task) - the task which caused the exception.
