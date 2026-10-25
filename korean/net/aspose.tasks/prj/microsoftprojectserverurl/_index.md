---
title: "Prj.MicrosoftProjectServerURL"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 프로젝트가 NT 사용자 대신 Project Server 사용자가 생성했는지 여부를 결정합니다"
type: docs
weight: 460
url: /ko/net/aspose.tasks/prj/microsoftprojectserverurl/
---
## Prj.MicrosoftProjectServerURL field

프로젝트가 NT 사용자 대신 Project Server 사용자에 의해 생성되었는지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, PrjKey> MicrosoftProjectServerURL;
```

## 예제

Prj.MicrosoftProjectServerURL 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.MicrosoftProjectServerURL, true);

Console.WriteLine("Microsoft Project Server U R L: " + project.Get(Prj.MicrosoftProjectServerURL));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


