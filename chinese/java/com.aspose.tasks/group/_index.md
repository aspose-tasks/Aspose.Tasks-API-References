---
title: "Group"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示组定义。"
type: docs
weight: 122
url: /zh/java/com.aspose.tasks/group/
---

**Inheritance:**
java.lang.Object
```
public class Group
```

表示组定义。Group 对象是 ResourceGroups 集合或 TaskGroups 集合的成员。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Group()](#Group--) | 初始化一个新的 [Group](../../com.aspose/tasks/group) 类实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getGroupAssignments()](#getGroupAssignments--) | 获取指示是否应将分配而不是任务进行分组的值。 |
| [getGroupCriteria()](#getGroupCriteria--) | 获取表示组定义中字段的 GroupCriteria 集合。 |
| [getMaintainHierarchy()](#getMaintainHierarchy--) | 获取指示是否在组内为子任务显示所有汇总任务层级的值。 |
| [getName()](#getName--) | 获取 Group 对象的名称。 |
| [getShowInMenu()](#getShowInMenu--) | 获取指示 Project 是否在功能区的 Group 下拉列表中显示组名称的值。 |
| [getShowSummary()](#getShowSummary--) | 获取指示是否为该组显示汇总行的值。 |
| [getUid()](#getUid--) | 获取组的唯一标识符。 |
| [setGroupAssignments(boolean value)](#setGroupAssignments-boolean-) | 设置指示是否应将分配而不是任务进行分组的值。 |
| [setGroupCriteria(GroupCriterionCollection value)](#setGroupCriteria-com.aspose.tasks.GroupCriterionCollection-) | 设置表示组定义中字段的 GroupCriteria 集合。 |
| [setMaintainHierarchy(boolean value)](#setMaintainHierarchy-boolean-) | 设置指示是否在组内为子任务显示所有汇总任务层级的值。 |
| [setName(String value)](#setName-java.lang.String-) | 设置 Group 对象的名称。 |
| [setShowInMenu(boolean value)](#setShowInMenu-boolean-) | 设置指示 Project 是否在功能区的 Group 下拉列表中显示组名称的值。 |
| [setShowSummary(boolean value)](#setShowSummary-boolean-) | 设置一个值，指示是否为该组显示汇总行。 |
### Group() {#Group--}
```
public Group()
```


初始化一个新的 [Group](../../com.aspose/tasks/group) 类实例。

### getGroupAssignments() {#getGroupAssignments--}
```
public final boolean getGroupAssignments()
```


获取指示是否应将分配而不是任务进行分组的值。

**Returns:**
boolean - 一个值，指示是否应将分配项分组而不是任务。
### getGroupCriteria() {#getGroupCriteria--}
```
public final GroupCriterionCollection getGroupCriteria()
```


获取表示组定义中字段的 GroupCriteria 集合。

**Returns:**
[GroupCriterionCollection](../../com.aspose.tasks/groupcriterioncollection) - a GroupCriteria collection representing the fields in a group definition.
### getMaintainHierarchy() {#getMaintainHierarchy--}
```
public final boolean getMaintainHierarchy()
```


获取指示是否在组内为子任务显示所有汇总任务层级的值。

**Returns:**
boolean - 一个值，指示是否在组内为子任务显示所有层级的汇总任务。
### getName() {#getName--}
```
public final String getName()
```


获取 Group 对象的名称。

**Returns:**
java.lang.String - 一个 Group 对象的名称。
### getShowInMenu() {#getShowInMenu--}
```
public final boolean getShowInMenu()
```


获取指示 Project 是否在功能区的 Group 下拉列表中显示组名称的值。

**Returns:**
boolean - 一个值，指示 Project 是否在功能区的 Group 下拉列表中显示组名称。
### getShowSummary() {#getShowSummary--}
```
public final boolean getShowSummary()
```


获取指示是否为该组显示汇总行的值。

**Returns:**
boolean - 一个值，指示是否为该组显示汇总行。
### getUid() {#getUid--}
```
public final int getUid()
```


获取组的唯一标识符。

**Returns:**
int - 一个组的唯一标识符。
### setGroupAssignments(boolean value) {#setGroupAssignments-boolean-}
```
public final void setGroupAssignments(boolean value)
```


设置指示是否应将分配而不是任务进行分组的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 一个值，指示是否应将分配项分组而不是任务。 |

### setGroupCriteria(GroupCriterionCollection value) {#setGroupCriteria-com.aspose.tasks.GroupCriterionCollection-}
```
public final void setGroupCriteria(GroupCriterionCollection value)
```


设置表示组定义中字段的 GroupCriteria 集合。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [GroupCriterionCollection](../../com.aspose.tasks/groupcriterioncollection) | 一个 GroupCriteria 集合，表示组定义中的字段。 |

### setMaintainHierarchy(boolean value) {#setMaintainHierarchy-boolean-}
```
public final void setMaintainHierarchy(boolean value)
```


设置指示是否在组内为子任务显示所有汇总任务层级的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 一个值，指示是否在组内为子任务显示所有层级的汇总任务。 |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


设置 Group 对象的名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 一个 Group 对象的名称。 |

### setShowInMenu(boolean value) {#setShowInMenu-boolean-}
```
public final void setShowInMenu(boolean value)
```


设置指示 Project 是否在功能区的 Group 下拉列表中显示组名称的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 一个值，指示 Project 是否在功能区的 Group 下拉列表中显示组名称。 |

### setShowSummary(boolean value) {#setShowSummary-boolean-}
```
public final void setShowSummary(boolean value)
```


设置一个值，指示是否为该组显示汇总行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 一个值，指示是否为该组显示汇总行。 |

