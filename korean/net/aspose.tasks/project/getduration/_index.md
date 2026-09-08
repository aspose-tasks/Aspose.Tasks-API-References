---
title: "Project.GetDuration"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 메서드. 지정된 단위 수와 프로젝트 설정인 DurationFormat에 정의된 기본 기간 형식으로 Duration 객체를 가져옵니다."
type: docs
weight: 1100
url: /ko/net/aspose.tasks/project/getduration/
---
## GetDuration(double) {#getduration}

[`Duration`](../../duration/) 객체를 지정된 단위 수와 프로젝트 설정인 [`DurationFormat`](../../prj/durationformat/)에 정의된 기본 기간 형식으로 가져옵니다.

```csharp
public Duration GetDuration(double val)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | Double | 지정된 단위 수. |

### 반환 값

Duration 객체.

## 비고

이 메서드는 Project.DurationFormat 설정에 따라 다른 기간을 반환하므로 주의해서 사용해야 합니다. 예를 들어, GetWork(1.0)은 Project.DurationFormat이 TimeUnitType.Hour인 경우 1시간을, TimeUnitType.Day인 경우 1일을 반환합니다.

## 예제

프로젝트 패브릭 메서드를 사용하여 기본 프로젝트 기간 형식으로 &lt;see cref=\"Aspose.Tasks.Duration\" /&gt; 인스턴스를 만드는 방법을 보여줍니다.

```csharp
var project = new Project();

// 기본 프로젝트 형식으로 기간을 가져옵니다.
var duration = project.GetDuration(1);

Console.WriteLine("Default project duration time unit type: " + project.Get(Prj.DurationFormat));
Console.WriteLine("Created duration time unit type: " + duration.TimeUnit);
```

### 또 보기

* struct [Duration](../../duration/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetDuration(double, TimeUnitType) {#getduration_1}

[`Duration`](../../duration/) 객체를 지정된 수의 [`TimeUnitType`](../../timeunittype/) 단위로 가져옵니다.

```csharp
public Duration GetDuration(double val, TimeUnitType timeUnit)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | Double | 지정된 단위 수. |
| timeUnit | TimeUnitType | 지정된 TimeUnitType 값. |

### 반환 값

Duration 객체.

## 예제

프로젝트 패브릭 메서드를 사용하여 &lt;see cref=\"Aspose.Tasks.Duration\" /&gt; 인스턴스를 만드는 방법을 보여줍니다.

```csharp
var project = new Project();

// 기본 프로젝트 형식으로 기간을 가져옵니다.
var duration = project.GetDuration(1, TimeUnitType.Minute);

Console.WriteLine("Created duration: " + duration);
```

### 또 보기

* struct [Duration](../../duration/)
* enum [TimeUnitType](../../timeunittype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetDuration(TimeSpan, TimeUnitType) {#getduration_2}

[`Duration`](../../duration/) 객체를 지정된 TimeSpan 값과 지정된 [`TimeUnitType`](../../timeunittype/) 값으로 가져옵니다.

```csharp
public Duration GetDuration(TimeSpan timeSpan, TimeUnitType timeUnit)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| timeSpan | TimeSpan | 지정된 TimeSpan 값. |
| timeUnit | TimeUnitType | 지정된 TimeUnitType 값. |

### 반환 값

Duration 객체.

### 또 보기

* struct [Duration](../../duration/)
* enum [TimeUnitType](../../timeunittype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


