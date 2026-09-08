---
title: "Project.Set"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 메서드. 지정된 속성을 이 컨테이너의 지정된 값에 매핑합니다."
type: docs
weight: 1240
url: /ko/net/aspose.tasks/project/set/
---
## Set&lt;T&gt;(Key&lt;T, PrjKey&gt;, T) {#set_1}

이 컨테이너에서 지정된 속성을 지정된 값에 매핑합니다.

```csharp
public void Set<T>(Key<T, PrjKey> key, T val)
```

| 매개변수 | 설명 |
| --- | --- |
| T | 매핑된 값의 유형. |
| key | 지정된 속성 키. [`Prj`](../../prj/)는 속성 키를 가져오기 위해 사용됩니다. |
| 값 | 값입니다. |

## 예제

작업 속성을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Set(Key&lt;DateTime, PrjKey&gt;, DateTime) {#set}

이 컨테이너에서 지정된 속성을 지정된 값에 매핑합니다.

```csharp
public void Set(Key<DateTime, PrjKey> key, DateTime val)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| key | Key`2 | 지정된 속성 키. [`Prj`](../../prj/)는 속성 키를 가져오기 위해 사용됩니다. |
| 값 | DateTime | 값입니다. |

## 예제

작업 속성을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


