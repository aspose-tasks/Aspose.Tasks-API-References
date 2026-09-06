---
title: "License.License"
second_title: "Aspose.Tasks for .NET API 参考"
description: "License 构造函数。初始化 License 类的新实例"
type: docs
weight: 10
url: /zh/net/aspose.tasks/license/license/
---
## License constructor

初始化 [`License`](../) 类的新实例。

```csharp
public License()
```

## 示例

在此示例中，将尝试在包含组件的文件夹、包含调用程序集的文件夹、入口程序集的文件夹以及调用程序集的嵌入资源中查找名为 MyLicense.lic 的许可证文件。

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

组件 jar 文件：

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

展示如何为 Aspose.Tasks 应用许可证。

```csharp
var license = new License();
license.SetLicense("Aspose.Tasks.lic");
```

### 另见

* class [License](../)
* namespace [Aspose.Tasks](../../license/)
* assembly [Aspose.Tasks](../../../)


