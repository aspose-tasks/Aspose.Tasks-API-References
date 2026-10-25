---
title: "TableTextStyle.TableTextStyle"
second_title: "Aspose.Tasks for .NET API 参考"
description: "TableTextStyle 构造函数。初始化 TableTextStyle 类的新实例。"
type: docs
weight: 10
url: /zh/net/aspose.tasks.visualization/tabletextstyle/tabletextstyle/
---
## TableTextStyle(int) {#constructor}

初始化 [`TableTextStyle`](../) 类的新实例。

```csharp
public TableTextStyle(int rowUid)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowUid | Int32 | 指定的行唯一标识。 |

## 示例

展示如何自定义表格文本样式，这些样式用于为项目中的不同文本项设置样式。

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.NewTasksAreManual, false);

var view = (GanttChartView)project.Views.ToList()[0];

// 设置第一个任务名称文本样式
var style1 = new TableTextStyle(1);
// 设置要应用样式的字段。
style1.Field = Field.TaskName;
// 设置文本样式的 <see cref=\"P:Aspose.Tasks.Visualization.TextStyle.Font\" />。
style1.Font = new FontDescriptor("Impact", 12F, FontStyles.Bold | FontStyles.Italic);
// 设置文本样式字体的点大小。

// 设置第二个任务持续时间文本样式
var style2 = new TableTextStyle(2);
style2.Field = Field.TaskDurationText;
style2.Font = new FontDescriptor("Impact", 16F, FontStyles.Underline);

view.TableTextStyles.Add(style1);
view.TableTextStyles.Add(style2);

SimpleSaveOptions options = new MPPSaveOptions
{
    // 设置指示必须写入视图数据的标志
    WriteViewData = true
};
project.Save(OutDir + "WorkWithTableTextStyle_out.mpp", options);
```

### 另见

* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, FontDescriptor) {#constructor_1}

使用指定的字体初始化 [`TableTextStyle`](../) 类的新实例。

```csharp
public TableTextStyle(int rowUid, FontDescriptor font)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowUid | Int32 | 指定的行唯一标识。 |
| font | FontDescriptor | 文本样式所基于的字体。 |

### 另见

* class [FontDescriptor](../../fontdescriptor/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, float, FontStyles) {#constructor_3}

使用指定的字体大小和字体样式初始化 [`TableTextStyle`](../) 类的新实例。

```csharp
public TableTextStyle(int rowUid, float fontSize, FontStyles fontStyle)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowUid | Int32 | 指定的行唯一标识。 |
| fontSize | Single | 文本样式所基于的字体大小。 |
| fontStyle | FontStyles | 文本样式所基于的字体样式。 |

### 另见

* enum [FontStyles](../../fontstyles/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, FontStyles) {#constructor_2}

使用默认字体设置和指定的字体样式初始化 [`TableTextStyle`](../) 类的新实例。

```csharp
public TableTextStyle(int rowUid, FontStyles fontStyle)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowUid | Int32 | 指定的行唯一标识。 |
| fontStyle | FontStyles | 文本样式所基于的字体样式。 |

### 另见

* enum [FontStyles](../../fontstyles/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)


