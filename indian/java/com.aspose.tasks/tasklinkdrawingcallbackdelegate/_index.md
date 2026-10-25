---
title: "TaskLinkDrawingCallbackDelegate"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "गैंट चार्ट व्यू में कार्य लिंक रेंडर होने पर कॉल किया जाने वाला कॉलबैक का प्रतिनिधित्व करता है।"
type: docs
weight: 298
url: /hi/java/com.aspose.tasks/tasklinkdrawingcallbackdelegate/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.Delegate, com.aspose.ms.System.MulticastDelegate
```
public abstract class TaskLinkDrawingCallbackDelegate extends System.MulticastDelegate
```

गैंट चार्ट व्यू में कार्य लिंक रेंडर होने पर कॉल किया जाने वाला कॉलबैक का प्रतिनिधित्व करता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [TaskLinkDrawingCallbackDelegate()](#TaskLinkDrawingCallbackDelegate--) |  |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [invoke(TaskLinkDrawingArgs args)](#invoke-com.aspose.tasks.TaskLinkDrawingArgs-) | टास्क लिंक ड्रॉइंग इवेंट को संभालने के लिए मेथड कॉलबैक को दर्शाता है। |
### TaskLinkDrawingCallbackDelegate() {#TaskLinkDrawingCallbackDelegate--}
```
public TaskLinkDrawingCallbackDelegate()
```


### invoke(TaskLinkDrawingArgs args) {#invoke-com.aspose.tasks.TaskLinkDrawingArgs-}
```
public abstract void invoke(TaskLinkDrawingArgs args)
```


टास्क लिंक ड्रॉइंग इवेंट को संभालने के लिए मेथड कॉलबैक को दर्शाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| args | [TaskLinkDrawingArgs](../../com.aspose.tasks/tasklinkdrawingargs) | [TaskLinkDrawingArgs](../../com.aspose.tasks/tasklinkdrawingargs) क्लास का वह उदाहरण जो कॉलबैक डेटा रखता है। |

