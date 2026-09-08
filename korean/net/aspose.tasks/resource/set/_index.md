---
title: "Resource.Set"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Resource 메서드. 지정된 속성을 이 컨테이너의 지정된 값에 매핑합니다"
type: docs
weight: 860
url: /ko/net/aspose.tasks/resource/set/
---
## Set&lt;T&gt;(Key&lt;T, RscKey&gt;, T) {#set_1}

이 컨테이너에서 지정된 속성을 지정된 값에 매핑합니다.

```csharp
public void Set<T>(Key<T, RscKey> key, T val)
```

| 매개변수 | 설명 |
| --- | --- |
| T | 매핑된 값의 유형. |
| key | 지정된 속성 키. [`Rsc`](../../rsc/)를 사용하여 속성 키를 가져옵니다. |
| 값 | 값입니다. |

## 예제

공통 리소스 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "UpdateResourceData.mpp");

// 리소스를 추가하고 일부 속성을 설정합니다
var resource = project.Resources.Add("Rsc");
resource.Set(Rsc.Start, new DateTime(2020, 4, 1, 8, 0, 0));
resource.Set(Rsc.StandardRate, 30);
resource.Set(Rsc.OvertimeRate, 45);
resource.Set(Rsc.Group, "Workgroup1");

Console.WriteLine("Resource Start: " + resource.Get(Rsc.Start));
Console.WriteLine("Resource Standard Rate: " + resource.Get(Rsc.StandardRate));
Console.WriteLine("Resource Overtime Rate: " + resource.Get(Rsc.OvertimeRate));
Console.WriteLine("Resource Group: " + resource.Get(Rsc.Group));

project.Save(OutDir + "UpdateResourceData_out.mpp", SaveFileFormat.Mpp);
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)

---

## Set(Key&lt;DateTime, RscKey&gt;, DateTime) {#set}

이 컨테이너에서 지정된 속성을 지정된 값에 매핑합니다.

```csharp
public void Set(Key<DateTime, RscKey> key, DateTime val)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| key | Key`2 | 지정된 속성 키. [`Rsc`](../../rsc/)를 사용하여 속성 키를 가져옵니다. |
| 값 | DateTime | 값입니다. |

## 예제

공통 리소스 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "UpdateResourceData.mpp");

// 리소스를 추가하고 일부 속성을 설정합니다
var resource = project.Resources.Add("Rsc");
resource.Set(Rsc.Start, new DateTime(2020, 4, 1, 8, 0, 0));
resource.Set(Rsc.StandardRate, 30);
resource.Set(Rsc.OvertimeRate, 45);
resource.Set(Rsc.Group, "Workgroup1");

Console.WriteLine("Resource Start: " + resource.Get(Rsc.Start));
Console.WriteLine("Resource Standard Rate: " + resource.Get(Rsc.StandardRate));
Console.WriteLine("Resource Overtime Rate: " + resource.Get(Rsc.OvertimeRate));
Console.WriteLine("Resource Group: " + resource.Get(Rsc.Group));

project.Save(OutDir + "UpdateResourceData_out.mpp", SaveFileFormat.Mpp);
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


