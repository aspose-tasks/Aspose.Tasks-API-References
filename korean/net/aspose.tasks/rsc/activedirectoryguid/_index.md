---
title: "Rsc.ActiveDirectoryGuid"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 리소스에 대한 Active Directory Guid"
type: docs
weight: 20
url: /ko/net/aspose.tasks/rsc/activedirectoryguid/
---
## Rsc.ActiveDirectoryGuid field

리소스에 대한 Active Directory Guid입니다.

```csharp
public static readonly Key<string, RscKey> ActiveDirectoryGuid;
```

## 예제

Rsc.ActiveDirectoryGuid 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActiveDirectoryGuid, "8aede269-c574-4a8b-aa74-32bc877a2aef");

Console.WriteLine("Active Directory Guid: " + resource.Get(Rsc.ActiveDirectoryGuid));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


