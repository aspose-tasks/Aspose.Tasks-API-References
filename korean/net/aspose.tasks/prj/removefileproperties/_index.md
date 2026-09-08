---
title: "Prj.RemoveFileProperties"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 저장 시 모든 파일 속성을 제거할지 여부를 결정합니다"
type: docs
weight: 600
url: /ko/net/aspose.tasks/prj/removefileproperties/
---
## Prj.RemoveFileProperties field

저장 시 모든 파일 속성이 제거되는지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, PrjKey> RemoveFileProperties;
```

## 예제

Prj.RemoveFileProperties 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.RemoveFileProperties, true);

Console.WriteLine("Remove File Properties: " + project.Get(Prj.RemoveFileProperties));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


