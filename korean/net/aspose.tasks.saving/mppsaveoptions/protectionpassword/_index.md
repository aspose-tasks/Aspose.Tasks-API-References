---
title: "MPPSaveOptions.ProtectionPassword"
second_title: "Aspose.Tasks for .NET API 참조"
description: "MPPSaveOptions 속성. 결과 MPP 파일을 보호하는 데 사용되는 비밀번호를 가져오거나 설정합니다. 현재 MS Project 2010 이상 형식에서 지원됩니다. null 값은 프로젝트 파일이 보호되지 않음을 나타냅니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks.saving/mppsaveoptions/protectionpassword/
---
## MPPSaveOptions.ProtectionPassword property

결과 MPP 파일을 보호하는 데 사용되는 비밀번호를 가져오거나 설정합니다. 현재 MS Project 2010 및 이후 형식에서 지원됩니다. null 값은 프로젝트 파일이 보호되지 않음을 나타냅니다.

```csharp
public string ProtectionPassword { get; set; }
```

## 예제

프로젝트를 비밀번호로 보호된 MPP 파일에 저장하는 방법을 보여줍니다.

```csharp
try
{

    var project = new Project(DataDir + "Project1.mpp");

    SimpleSaveOptions options = new MPPSaveOptions
    {
        ProtectionPassword = "password!234"
    };

    project.Save(OutDir + "PasswordProtected.mpp", options);
}
catch (NotSupportedException ex)
{
    Console.WriteLine(ex.Message + "\nThis example will only work if you apply a valid Aspose License. You can purchase full license or get 30 day temporary license from http://www.aspose.com/purchase/default.aspx.");
}
```

### 또 보기

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


