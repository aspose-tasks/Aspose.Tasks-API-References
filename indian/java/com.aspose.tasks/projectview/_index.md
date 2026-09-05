---
title: "ProjectView"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "Projects व्यू क्लास"
type: docs
weight: 228
url: /hi/java/com.aspose.tasks/projectview/
---

**Inheritance:**
java.lang.Object
```
public class ProjectView
```

प्रोजेक्ट का दृश्य वर्ग
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [ProjectView(Iterable&lt;ViewColumn&gt; columns)](#ProjectView-java.lang.Iterable-com.aspose.tasks.ViewColumn--) | [ProjectView](../../com.aspose.tasks/projectview) वर्ग की नई इंस्टेंस को प्रारंभ करता है। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getColumns()](#getColumns--) | प्रोजेक्ट व्यू कॉलम प्राप्त करता है। |
| [getDefaultAssignmentView()](#getDefaultAssignmentView--) | Uid, कार्य नाम, संसाधन नाम, कार्य और अवधि असाइनमेंट कॉलम शामिल करता है। |
| [getDefaultGanttChartView()](#getDefaultGanttChartView--) | id, संकेतक, नाम, अवधि, प्रारंभ और समाप्ति कार्य स्तंभ शामिल हैं। |
| [getDefaultResourceSheetView()](#getDefaultResourceSheetView--) | Uid, संसाधन नाम, प्रकार, सामग्री लेबल, प्रारंभिक अक्षर, समूह, अधिकतम इकाइयाँ, मानक दर, ओवरटाइम दर, उपयोग प्रति लागत, संचित समय, आधार कैलेंडर और कोड संसाधन स्तंभ शामिल हैं। |
| [getDefaultResourceUsageView()](#getDefaultResourceUsageView--) | Uid, नाम, प्रारंभ, समाप्ति और कार्य संसाधन स्तंभ शामिल हैं। |
| [getDefaultTaskSheetView()](#getDefaultTaskSheetView--) | id, संकेतक, नाम, अवधि, प्रारंभ, समाप्ति, पूर्ववर्ती और संसाधन नाम कार्य स्तंभ शामिल हैं। |
### ProjectView(Iterable&lt;ViewColumn&gt; columns) {#ProjectView-java.lang.Iterable-com.aspose.tasks.ViewColumn--}
```
public ProjectView(Iterable<ViewColumn> columns)
```


[ProjectView](../../com.aspose.tasks/projectview) वर्ग की नई इंस्टेंस को प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| स्तंभ | java.lang.Iterable&lt;com.aspose.tasks.ViewColumn&gt; | दृश्य स्तंभों की एक सूची। |

### getColumns() {#getColumns--}
```
public final List<ViewColumn> getColumns()
```


प्रोजेक्ट व्यू कॉलम प्राप्त करता है।

**Returns:**
java.util.List&lt;com.aspose.tasks.ViewColumn&gt; - प्रोजेक्ट दृश्य स्तंभ।
### getDefaultAssignmentView() {#getDefaultAssignmentView--}
```
public static ProjectView getDefaultAssignmentView()
```


Uid, कार्य नाम, संसाधन नाम, कार्य और अवधि असाइनमेंट कॉलम शामिल करता है।

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn).
### getDefaultGanttChartView() {#getDefaultGanttChartView--}
```
public static ProjectView getDefaultGanttChartView()
```


id, संकेतक, नाम, अवधि, प्रारंभ और समाप्ति कार्य स्तंभ शामिल हैं।

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn).
### getDefaultResourceSheetView() {#getDefaultResourceSheetView--}
```
public static ProjectView getDefaultResourceSheetView()
```


Uid, संसाधन नाम, प्रकार, सामग्री लेबल, प्रारंभिक अक्षर, समूह, अधिकतम इकाइयाँ, मानक दर, ओवरटाइम दर, उपयोग प्रति लागत, संचित समय, आधार कैलेंडर और कोड संसाधन स्तंभ शामिल हैं।

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).
### getDefaultResourceUsageView() {#getDefaultResourceUsageView--}
```
public static ProjectView getDefaultResourceUsageView()
```


Uid, नाम, प्रारंभ, समाप्ति और कार्य संसाधन स्तंभ शामिल हैं।

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).
### getDefaultTaskSheetView() {#getDefaultTaskSheetView--}
```
public static ProjectView getDefaultTaskSheetView()
```


id, संकेतक, नाम, अवधि, प्रारंभ, समाप्ति, पूर्ववर्ती और संसाधन नाम कार्य स्तंभ शामिल हैं।

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn).
