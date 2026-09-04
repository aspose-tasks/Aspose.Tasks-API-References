---
title: "ProjectView"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "فئة عرض المشاريع"
type: docs
weight: 228
url: /ar/java/com.aspose.tasks/projectview/
---

**Inheritance:**
java.lang.Object
```
public class ProjectView
```

فئة عرض المشروع
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [ProjectView(Iterable&lt;ViewColumn&gt; columns)](#ProjectView-java.lang.Iterable-com.aspose.tasks.ViewColumn--) | ينشئ مثيلاً جديداً من الفئة [ProjectView](../../com.aspose.tasks/projectview). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getColumns()](#getColumns--) | يحصل على أعمدة عرض المشروع. |
| [getDefaultAssignmentView()](#getDefaultAssignmentView--) | يتضمن أعمدة UID، اسم المهمة، اسم المورد، العمل ومدة التعيين. |
| [getDefaultGanttChartView()](#getDefaultGanttChartView--) | يتضمن id، المؤشرات، الاسم، المدة، بدء وانتهاء أعمدة المهمة. |
| [getDefaultResourceSheetView()](#getDefaultResourceSheetView--) | يتضمن Uid، اسم المورد، النوع، تسمية المادة، الأحرف الأولى، المجموعة، الحد الأقصى للوحدات، السعر القياسي، سعر العمل الإضافي، التكلفة لكل استخدام، التراكم في، التقويم الأساسي و أعمدة رمز المورد. |
| [getDefaultResourceUsageView()](#getDefaultResourceUsageView--) | يتضمن Uid، الاسم، بدء، انتهاء و أعمدة مورد العمل. |
| [getDefaultTaskSheetView()](#getDefaultTaskSheetView--) | يتضمن id، المؤشرات، الاسم، المدة، بدء، انتهاء، السلفيات وأسماء الموارد أعمدة المهمة. |
### ProjectView(Iterable&lt;ViewColumn&gt; columns) {#ProjectView-java.lang.Iterable-com.aspose.tasks.ViewColumn--}
```
public ProjectView(Iterable<ViewColumn> columns)
```


ينشئ مثيلاً جديداً من الفئة [ProjectView](../../com.aspose.tasks/projectview).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الأعمدة | java.lang.Iterable&lt;com.aspose.tasks.ViewColumn&gt; | قائمة بأعمدة العرض. |

### getColumns() {#getColumns--}
```
public final List<ViewColumn> getColumns()
```


يحصل على أعمدة عرض المشروع.

**Returns:**
java.util.List&lt;com.aspose.tasks.ViewColumn&gt; - أعمدة عرض المشروع.
### getDefaultAssignmentView() {#getDefaultAssignmentView--}
```
public static ProjectView getDefaultAssignmentView()
```


يتضمن أعمدة UID، اسم المهمة، اسم المورد، العمل ومدة التعيين.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn).
### getDefaultGanttChartView() {#getDefaultGanttChartView--}
```
public static ProjectView getDefaultGanttChartView()
```


يتضمن id، المؤشرات، الاسم، المدة، بدء وانتهاء أعمدة المهمة.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn).
### getDefaultResourceSheetView() {#getDefaultResourceSheetView--}
```
public static ProjectView getDefaultResourceSheetView()
```


يتضمن Uid، اسم المورد، النوع، تسمية المادة، الأحرف الأولى، المجموعة، الحد الأقصى للوحدات، السعر القياسي، سعر العمل الإضافي، التكلفة لكل استخدام، التراكم في، التقويم الأساسي و أعمدة رمز المورد.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).
### getDefaultResourceUsageView() {#getDefaultResourceUsageView--}
```
public static ProjectView getDefaultResourceUsageView()
```


يتضمن Uid، الاسم، بدء، انتهاء و أعمدة مورد العمل.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).
### getDefaultTaskSheetView() {#getDefaultTaskSheetView--}
```
public static ProjectView getDefaultTaskSheetView()
```


يتضمن id، المؤشرات، الاسم، المدة، بدء، انتهاء، السلفيات وأسماء الموارد أعمدة المهمة.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn).
