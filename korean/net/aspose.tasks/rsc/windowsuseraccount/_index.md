---
title: "Rsc.WindowsUserAccount"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 리소스와 연결된 NT 계정"
type: docs
weight: 680
url: /ko/net/aspose.tasks/rsc/windowsuseraccount/
---
## Rsc.WindowsUserAccount field

리소스와 연결된 NT 계정.

```csharp
public static readonly Key<string, RscKey> WindowsUserAccount;
```

## 예제

리소스의 메타 속성을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project.mpp");

// 리소스를 추가하고 리소스 메타 데이터를 설정합니다.
var resource = project.Resources.Add("Rsc 1");
resource.Set(Rsc.EMailAddress, "1@gmail.com");
resource.Set(Rsc.WindowsUserAccount, "user_acc1");
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


