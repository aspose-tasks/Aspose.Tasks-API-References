---
title: "LoadOptions.Password"
second_title: "Aspose.Tasks for .NET API 참조"
description: "LoadOptions 속성. 보호 비밀번호를 가져오거나 설정합니다."
type: docs
weight: 50
url: /ko/net/aspose.tasks/loadoptions/password/
---
## LoadOptions.Password property

보호 비밀번호를 가져오거나 설정합니다.

```csharp
public string Password { get; set; }
```

## 예제

<see cref="Aspose.Tasks.LoadOptions"/> 인스턴스를 사용하여 비밀번호로 보호된 프로젝트를 로드하는 방법을 보여줍니다.

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var options = new LoadOptions
    {
        Password = "password"
    };
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### 또 보기

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


