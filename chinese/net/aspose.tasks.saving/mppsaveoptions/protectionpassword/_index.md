---
title: "MPPSaveOptions.ProtectionPassword"
second_title: "Aspose.Tasks for .NET API 参考"
description: "MPPSaveOptions 属性。获取或设置用于保护生成的 MPP 文件的密码。当前支持 MS Project 2010 及更高版本的格式。空值表示项目文件未受保护。"
type: docs
weight: 30
url: /zh/net/aspose.tasks.saving/mppsaveoptions/protectionpassword/
---
## MPPSaveOptions.ProtectionPassword property

获取或设置用于保护生成的 MPP 文件的密码。当前支持 MS Project 2010 及更高版本的格式。空值表示项目文件未受保护。

```csharp
public string ProtectionPassword { get; set; }
```

## 示例

展示如何将项目保存为受密码保护的 MPP 文件。

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

### 另见

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


