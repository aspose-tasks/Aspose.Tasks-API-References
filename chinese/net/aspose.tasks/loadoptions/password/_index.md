---
title: "LoadOptions.Password"
second_title: "Aspose.Tasks for .NET API 参考"
description: "LoadOptions 属性。获取或设置保护密码。"
type: docs
weight: 50
url: /zh/net/aspose.tasks/loadoptions/password/
---
## LoadOptions.Password property

获取或设置保护密码。

```csharp
public string Password { get; set; }
```

## 示例

展示如何使用 &lt;see cref="Aspose.Tasks.LoadOptions"/&gt; 实例加载受密码保护的项目。

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

### 另见

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


