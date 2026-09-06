---
title: "Metered.GetConsumptionQuantity"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Metered 方法。获取消费文件大小"
type: docs
weight: 60
url: /zh/net/aspose.tasks/metered/getconsumptionquantity/
---
## Metered.GetConsumptionQuantity method

获取消耗文件大小。

```csharp
public static decimal GetConsumptionQuantity()
```

### 返回值

返回已消耗的字节数。

## 示例

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

* class [Metered](../)
* namespace [Aspose.Tasks](../../metered/)
* assembly [Aspose.Tasks](../../../)


