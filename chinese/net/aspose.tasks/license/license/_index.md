---
title: License
second_title: Aspose.Tasks for .NET API 参考
description: 初始化Licenseaspose.tasks/license类的新实例
type: docs
weight: 10
url: /zh/net/aspose.tasks/license/license/
---
## License constructor

初始化[`License`](../../license)类的新实例。

```csharp
public License()
```

### 例子

在本例中，将尝试查找名为 MyLicense.lic 的许可证文件在包含 的文件夹中 组件 在包含调用程序集的文件夹中 在入口程序集的文件夹中，然后在调用程序集的嵌入资源中。

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

组件 jar 文件:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

### 也可以看看

* class [License](../../license)
* 命名空间 [Aspose.Tasks](../../license)
* 部件 [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
