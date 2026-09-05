---
title: "ITextStyleModificationCallback"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "टेबल सेल पर TextStyle लागू होने से पहले कॉल किया जाने वाला कॉलबैक दर्शाता है।"
type: docs
weight: 383
url: /hi/java/com.aspose.tasks/itextstylemodificationcallback/
---
```
public interface ITextStyleModificationCallback
```

टेबल सेल पर TextStyle लागू होने से पहले कॉल किया जाने वाला कॉलबैक दर्शाता है।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [beforeTaskTextStyleApplied(TaskTextStyleEventArgs args)](#beforeTaskTextStyleApplied-com.aspose.tasks.TaskTextStyleEventArgs-) | टेबल सेल को रेंडर करने से पहले कार्य पंक्ति के लिए कॉल की जाने वाली विधि निम्नलिखित दृश्यों में: 'Gantt Chart', 'Task Sheet', 'Task Usage'। |
### beforeTaskTextStyleApplied(TaskTextStyleEventArgs args) {#beforeTaskTextStyleApplied-com.aspose.tasks.TaskTextStyleEventArgs-}
```
public abstract void beforeTaskTextStyleApplied(TaskTextStyleEventArgs args)
```


टेबल सेल को रेंडर करने से पहले कार्य पंक्ति के लिए कॉल की जाने वाली विधि निम्नलिखित दृश्यों में: 'Gantt Chart', 'Task Sheet', 'Task Usage'।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| args | [TaskTextStyleEventArgs](../../com.aspose.tasks/tasktextstyleeventargs) | यह [TaskTextStyleEventArgs](../../com.aspose.tasks/tasktextstyleeventargs) ऑब्जेक्ट। |

