---
title: "Project.GetDuration"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 方法。获取具有指定单位数和默认持续时间格式的 Duration 对象，该格式在项目设置 DurationFormat 中定义。"
type: docs
weight: 1100
url: /zh/net/aspose.tasks/project/getduration/
---
## GetDuration(double) {#getduration}

获取 [`Duration`](../../duration/) 对象，具有指定的单位数和默认持续时间格式，该格式在项目设置 [`DurationFormat`](../../prj/durationformat/) 中定义。

```csharp
public Duration GetDuration(double val)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| val | Double | 指定的单位数。 |

### 返回值

Duration 对象。

## 备注

此方法应谨慎使用，因为它会根据 Project.DurationFormat 设置返回不同的持续时间。例如，当 Project.DurationFormat 为 TimeUnitType.Hour 时，GetWork(1.0) 将返回 1 小时；如果 Project.DurationFormat 为 TimeUnitType.Day，则返回 1 天。

## 示例

展示如何使用项目工厂方法创建一个 &lt;see cref="Aspose.Tasks.Duration" /&gt; 实例，使用默认项目的持续时间格式。

```csharp
var project = new Project();

// 获取使用默认项目格式的持续时间。
var duration = project.GetDuration(1);

Console.WriteLine("Default project duration time unit type: " + project.Get(Prj.DurationFormat));
Console.WriteLine("Created duration time unit type: " + duration.TimeUnit);
```

### 另见

* struct [Duration](../../duration/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetDuration(double, TimeUnitType) {#getduration_1}

获取 [`Duration`](../../duration/) 对象，具有指定数量的 [`TimeUnitType`](../../timeunittype/) 单位。

```csharp
public Duration GetDuration(double val, TimeUnitType timeUnit)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| val | Double | 指定的单位数。 |
| timeUnit | TimeUnitType | 指定的 TimeUnitType 值。 |

### 返回值

Duration 对象。

## 示例

展示如何使用项目工厂方法创建一个 &lt;see cref="Aspose.Tasks.Duration" /&gt; 实例。

```csharp
var project = new Project();

// 获取使用默认项目格式的持续时间。
var duration = project.GetDuration(1, TimeUnitType.Minute);

Console.WriteLine("Created duration: " + duration);
```

### 另见

* struct [Duration](../../duration/)
* enum [TimeUnitType](../../timeunittype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetDuration(TimeSpan, TimeUnitType) {#getduration_2}

获取 [`Duration`](../../duration/) 对象，使用指定的 TimeSpan 值和指定的 [`TimeUnitType`](../../timeunittype/) 值。

```csharp
public Duration GetDuration(TimeSpan timeSpan, TimeUnitType timeUnit)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| timeSpan | TimeSpan | 指定的 TimeSpan 值。 |
| timeUnit | TimeUnitType | 指定的 TimeUnitType 值。 |

### 返回值

Duration 对象。

### 另见

* struct [Duration](../../duration/)
* enum [TimeUnitType](../../timeunittype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


