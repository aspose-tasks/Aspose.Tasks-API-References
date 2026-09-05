---
title: "TaskTextStyleEventArgs"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "यह क्लास तालिका कोशिकाओं की सामग्री के रेंडरिंग से संबंधित डेटा का सेट दर्शाती है।"
type: docs
weight: 302
url: /hi/java/com.aspose.tasks/tasktextstyleeventargs/
---

**Inheritance:**
java.lang.Object
```
public class TaskTextStyleEventArgs
```

यह क्लास तालिका सेल की सामग्री के रेंडरिंग से संबंधित डेटा सेट का प्रतिनिधित्व करती है।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getCellTextStyle()](#getCellTextStyle--) | सेल की सामग्री को ड्रॉ करने के लिए उपयोग किया जाने वाला TextStyle प्राप्त करता है। |
| [getColumn()](#getColumn--) | वर्तमान में रेंडर किए जा रहे सेल से संबंधित [ViewColumn](../../com.aspose.tasks/viewcolumn) प्राप्त करता है। |
| [getTask()](#getTask--) | वर्तमान में रेंडर की गई पंक्ति से संबंधित `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) प्राप्त करता है। |
| [setCellTextStyle(TextStyle value)](#setCellTextStyle-com.aspose.tasks.TextStyle-) | सेल की सामग्री को ड्रॉ करने के लिए उपयोग किए जाने वाले TextStyle को सेट करता है। |
### getCellTextStyle() {#getCellTextStyle--}
```
public final TextStyle getCellTextStyle()
```


सेल की सामग्री को ड्रॉ करने के लिए उपयोग किए जाने वाले TextStyle को प्राप्त करता है। इस ऑब्जेक्ट का उपयोग तालिका सेल की उपस्थिति को अनुकूलित करने के लिए किया जा सकता है।

**Returns:**
[TextStyle](../../com.aspose.tasks/textstyle) - TextStyle which will be used to draw the cell's content.
### getColumn() {#getColumn--}
```
public final ViewColumn getColumn()
```


वर्तमान में रेंडर किए जा रहे सेल से संबंधित [ViewColumn](../../com.aspose.tasks/viewcolumn) प्राप्त करता है।

**Returns:**
[ViewColumn](../../com.aspose.tasks/viewcolumn) - [ViewColumn](../../com.aspose.tasks/viewcolumn) to which the currently rendered cell belongs.
### getTask() {#getTask--}
```
public final Task getTask()
```


वर्तमान में रेंडर की गई पंक्ति से संबंधित `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) प्राप्त करता है।

**Returns:**
[Task](../../com.aspose.tasks/task) - `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) which corresponds to the currently rendered row.
### setCellTextStyle(TextStyle value) {#setCellTextStyle-com.aspose.tasks.TextStyle-}
```
public final void setCellTextStyle(TextStyle value)
```


सेल की सामग्री को ड्रॉ करने के लिए उपयोग किए जाने वाले TextStyle को सेट करता है। इस ऑब्जेक्ट का उपयोग तालिका सेल की उपस्थिति को अनुकूलित करने के लिए किया जा सकता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [TextStyle](../../com.aspose.tasks/textstyle) | सेल की सामग्री को ड्रॉ करने के लिए उपयोग किया जाने वाला TextStyle। |

