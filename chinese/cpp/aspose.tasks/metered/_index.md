---
title: "Aspose::Tasks::Metered 类"
linktitle: "计量"
articleTitle: "计量"
second_title: "Aspose.Tasks for C++"
description: "提供设置计量密钥的方法。"
type: docs
weight: 10
url: /zh/cpp/aspose.tasks/metered/
---

## Metered class

提供设置计量密钥的方法。

在此示例中，将尝试设置计量的公钥和私钥 <ms>

```cpp
[C#]
 
Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");
 
 
[Visual Basic]
 
Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

</ms> <java> 组件 jar 文件：

```cpp
Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
```

</java>

## 方法

| 表示 ResourceAssignment 对象的属性。 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| [GetConsumptionCredit](./getconsumptioncredit/) | 获取消耗积分。 |
| [GetConsumptionQuantity](./getconsumptionquantity/) | 获取消耗文件大小。 |
| [IsLicensed](./islicensed/) | 检查产品是否使用计量许可证成功授权。 |
| [ResetMeteredKey](./resetmeteredkey/) | 移除先前设置的许可证。 |
| [SetMeteredKey](./setmeteredkey/) | 设置计量的公钥和私钥。 |

