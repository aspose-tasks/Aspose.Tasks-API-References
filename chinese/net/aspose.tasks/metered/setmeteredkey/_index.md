---
title: "Metered.SetMeteredKey"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Metered 方法。设置 Metered 公钥和私钥"
type: docs
weight: 40
url: /zh/net/aspose.tasks/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

设置计量公共和私有密钥。

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| publicKey | 字符串 | 公钥。 |
| privateKey | 字符串 | 私钥。 |

## 备注

如果您购买了计量许可证，应在应用程序启动时调用此 API，通常这已经足够。然而，如果计量在 24 小时内未能上传消费数据，许可证将被设置为评估状态。为避免这种情况，您应定期检查许可证状态；如果是评估状态，请再次调用此 API。

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


