---
title: "Project.SetBaseline"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 메서드. 전체 프로젝트에 대해 지정된 기준선에 기준선 필드를 저장합니다."
type: docs
weight: 1250
url: /ko/net/aspose.tasks/project/setbaseline/
---
## SetBaseline(BaselineType) {#setbaseline}

전체 프로젝트에 대해 지정된 기준선에 기준선 필드를 저장합니다.

```csharp
public void SetBaseline(BaselineType baselineType)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| baselineType | BaselineType | 기준선 데이터를 저장할 기준선 유형입니다. |

## 예제

전체 프로젝트에 대한 기준선을 만드는 방법을 보여줍니다.

```csharp
var project = new Project();

// 작업 추가
project.RootTask.Children.Add("Task");
project.RootTask.Children.Add("Task2");

// 지정된 작업에 대한 기준선을 설정합니다.
project.SetBaseline(BaselineType.Baseline);
```

### 또 보기

* enum [BaselineType](../../baselinetype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SetBaseline(BaselineType, IEnumerable&lt;Task&gt;) {#setbaseline_1}

선택된 작업에 대해 지정된 기준선에 기준선 필드를 저장합니다.

```csharp
public void SetBaseline(BaselineType baselineType, IEnumerable<Task> taskCollection)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| baselineType | BaselineType | 기준선 데이터를 저장할 기준선 유형입니다. |
| taskCollection | IEnumerable`1 | 기준선 데이터를 저장할 작업 목록입니다. |

## 예제

특정 작업에 대한 설정된 기준선을 만드는 방법을 보여줍니다.

```csharp
var project = new Project();

// 작업 추가
var task = project.RootTask.Children.Add("Task");
var task2 = project.RootTask.Children.Add("Task2");

// 지정된 작업에 대한 기준선을 설정합니다.
project.SetBaseline(BaselineType.Baseline, new[] { task, task2 });
```

### 또 보기

* enum [BaselineType](../../baselinetype/)
* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


