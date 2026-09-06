---
title: "类 Metered"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Metered 类。提供设置计量密钥的方法"
type: docs
weight: 1020
url: /zh/net/aspose.tasks/metered/
---
## Metered class

提供设置计量密钥的方法。

```csharp
public class Metered
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [Metered](metered/)() | 默认构造函数。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [IsLicensed](../../aspose.tasks/metered/islicensed/)() | 检查产品是否已使用计量许可证成功授权。 |
| [ResetMeteredKey](../../aspose.tasks/metered/resetmeteredkey/)() | 移除先前设置的许可证。 |
| [SetMeteredKey](../../aspose.tasks/metered/setmeteredkey/)(string, string) | 设置计量公共和私有密钥。 |
| static [GetConsumptionCredit](../../aspose.tasks/metered/getconsumptioncredit/)() | 获取消耗积分。 |
| static [GetConsumptionQuantity](../../aspose.tasks/metered/getconsumptionquantity/)() | 获取消耗文件大小。 |

## 示例

在此示例中，将尝试设置计量公共和私有密钥

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

组件 jar 文件：

```csharp
Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
```

展示如何使用 &lt;see cref="Aspose.Tasks.Metered" /&gt; 许可证类型与 Aspose.Tasks。

```csharp
// 让我们使用计量许可证（参见 https://purchase.aspose.com/faqs/licensing/metered）
// 设置计量许可证
var metered = new Metered();
metered.SetMeteredKey("<public key>", "<private key>");

var project = new Project(DataDir + "Project2.mpp");
Console.WriteLine("Project Name: " + project.Get(Prj.Name));

// ...
// 处理项目...
// ...

// 我们可以获取当前的积分和字节消耗。

try
{
    Console.WriteLine("Credits spent: {0}", Metered.GetConsumptionCredit());
    Console.WriteLine("Bytes consumed: {0}", Metered.GetConsumptionQuantity());
}
catch (WebException)
{
    // 记录异常
}

// 最近用户可以重置计量并停止字节计数
metered.ResetMeteredKey();
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


