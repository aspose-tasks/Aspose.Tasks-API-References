---
title: "Table"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示项目中的表。"
type: docs
weight: 284
url: /zh/java/com.aspose.tasks/table/
---

**Inheritance:**
java.lang.Object
```
public class Table
```

表示项目中的表。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Table()](#Table--) | 初始化 [Table](../../com.aspose.tasks/table) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | 返回一个值，指示此实例是否等于指定的对象。 |
| [getAdjustHeaderRowHeight()](#getAdjustHeaderRowHeight--) | 获取一个值，指示表的标题行高度是否可以调整。 |
| [getDateFormat()](#getDateFormat--) | 获取表的日期格式。 |
| [getLockFirstColumn()](#getLockFirstColumn--) | 获取一个值，指示表的第一列是锁定还是可编辑。 |
| [getName()](#getName--) | 获取 Table 对象的名称。 |
| [getRowHeight()](#getRowHeight--) | 获取表中行的高度，其中行高度是文本行数。 |
| [getShowAddNewColumn()](#getShowAddNewColumn--) | 获取一个值，指示是否显示 “Add New Column” 界面。 |
| [getShowInMenu()](#getShowInMenu--) | 获取一个值，指示项目是否在功能区 View 选项卡的 Tables 下拉列表中显示表名。 |
| [getTableFields()](#getTableFields--) | 获取表示表中字段的 TableFields 集合。 |
| [getTableType()](#getTableType--) | 获取指定表的表类型。 |
| [getUid()](#getUid--) | 获取表的唯一标识符。 |
| [hashCode()](#hashCode--) | 返回此 Table 的哈希码。 |
| [setAdjustHeaderRowHeight(boolean value)](#setAdjustHeaderRowHeight-boolean-) | 设置一个值，指示表的标题行高度是否可以调整。 |
| [setDateFormat(int value)](#setDateFormat-int-) | 设置表的日期格式。 |
| [setLockFirstColumn(boolean value)](#setLockFirstColumn-boolean-) | 设置一个值，指示表的第一列是锁定还是可编辑。 |
| [setName(String value)](#setName-java.lang.String-) | 设置 Table 对象的名称。 |
| [setRowHeight(int value)](#setRowHeight-int-) | 设置表中行的高度，其中行高度是文本行数。 |
| [setShowAddNewColumn(boolean value)](#setShowAddNewColumn-boolean-) | 设置一个值，指示是否显示 “Add New Column” 界面。 |
| [setShowInMenu(boolean value)](#setShowInMenu-boolean-) | 设置一个值，指示项目是否在功能区 View 选项卡的 Tables 下拉列表中显示表名。 |
| [setTableType(int value)](#setTableType-int-) | 设置指定表的表类型。 |
### Table() {#Table--}
```
public Table()
```


初始化 [Table](../../com.aspose.tasks/table) 类的新实例。

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


返回一个值，指示此实例是否等于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | java.lang.Object | 用于与此实例比较的对象。 |

**Returns:**
boolean - **True** 如果指定的对象是具有与此实例相同 UID 值的 Table；否则为 **false**。
### getAdjustHeaderRowHeight() {#getAdjustHeaderRowHeight--}
```
public final boolean getAdjustHeaderRowHeight()
```


获取一个值，指示表的标题行高度是否可以调整。

**Returns:**
boolean - 指示表的标题行高度是否可以调整的值。
### getDateFormat() {#getDateFormat--}
```
public final int getDateFormat()
```


获取表的日期格式。

**Returns:**
int - 表格的日期格式。
### getLockFirstColumn() {#getLockFirstColumn--}
```
public final boolean getLockFirstColumn()
```


获取一个值，指示表的第一列是锁定还是可编辑。

**Returns:**
boolean - 指示表格第一列是否被锁定或可编辑的值。
### getName() {#getName--}
```
public final String getName()
```


获取 Table 对象的名称。

**Returns:**
java.lang.String - Table 对象的名称。
### getRowHeight() {#getRowHeight--}
```
public final int getRowHeight()
```


获取表中行的高度，其中行高度是文本行数。

**Returns:**
int - 表格中行的高度，行高是文本行数。
### getShowAddNewColumn() {#getShowAddNewColumn--}
```
public final boolean getShowAddNewColumn()
```


获取一个值，指示是否显示 “Add New Column” 界面。

--------------------

支持 MSP 2010 版及更高版本。

**Returns:**
boolean - 指示是否显示 'Add New Column' 界面的值。
### getShowInMenu() {#getShowInMenu--}
```
public final boolean getShowInMenu()
```


获取一个值，指示项目是否在功能区 View 选项卡的 Tables 下拉列表中显示表名。

**Returns:**
boolean - 指示项目是否在功能区 View 选项卡的 Tables 下拉列表中显示表名的值。
### getTableFields() {#getTableFields--}
```
public final TableFieldCollection getTableFields()
```


获取表示表中字段的 TableFields 集合。

**Returns:**
[TableFieldCollection](../../com.aspose.tasks/tablefieldcollection) - a TableFields collection representing the fields in the table.
### getTableType() {#getTableType--}
```
public final int getTableType()
```


获取指定表的表类型。

**Returns:**
int - 指定表的表类型。
### getUid() {#getUid--}
```
public final int getUid()
```


获取表的唯一标识符。

**Returns:**
int - 表的唯一标识符。
### hashCode() {#hashCode--}
```
public int hashCode()
```


返回此 Table 的哈希码。

**Returns:**
int - 返回此对象的哈希码值。
### setAdjustHeaderRowHeight(boolean value) {#setAdjustHeaderRowHeight-boolean-}
```
public final void setAdjustHeaderRowHeight(boolean value)
```


设置一个值，指示表的标题行高度是否可以调整。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示表格标题行高度是否可调整的值。 |

### setDateFormat(int value) {#setDateFormat-int-}
```
public final void setDateFormat(int value)
```


设置表的日期格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 表格的日期格式。 |

### setLockFirstColumn(boolean value) {#setLockFirstColumn-boolean-}
```
public final void setLockFirstColumn(boolean value)
```


设置一个值，指示表的第一列是锁定还是可编辑。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示表格第一列是否被锁定或可编辑的值。 |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


设置 Table 对象的名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | Table 对象的名称。 |

### setRowHeight(int value) {#setRowHeight-int-}
```
public final void setRowHeight(int value)
```


设置表中行的高度，其中行高度是文本行数。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 表格中行的高度，行高是文本行数。 |

### setShowAddNewColumn(boolean value) {#setShowAddNewColumn-boolean-}
```
public final void setShowAddNewColumn(boolean value)
```


设置一个值，指示是否显示 “Add New Column” 界面。

--------------------

支持 MSP 2010 版及更高版本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示是否显示 'Add New Column' 界面的值。 |

### setShowInMenu(boolean value) {#setShowInMenu-boolean-}
```
public final void setShowInMenu(boolean value)
```


设置一个值，指示项目是否在功能区 View 选项卡的 Tables 下拉列表中显示表名。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示项目是否在功能区 View 选项卡的 Tables 下拉列表中显示表名的值。 |

### setTableType(int value) {#setTableType-int-}
```
public final void setTableType(int value)
```


设置指定表的表类型。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 指定表的表类型。 |

