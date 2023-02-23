---
title: Metered.SetMeteredKey
second_title: Aspose.Tasks for .NET API 参考
description: Metered 方法. 设置计量公钥和私钥
type: docs
weight: 30
url: /zh/net/aspose.tasks/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

设置计量公钥和私钥。

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| publicKey | String | 公钥。 |
| privateKey | String | 私钥。 |

### 评论

如果你购买了metered license，这个API应该在应用程序启动时调用，正常情况下，这就足够了。 但是，如果metered在24小时内没有上传消费数据，那么license将被设置为评估状态。为避免这种情况，您应该定期检查许可证状态。如果是评估状态，请再次调用此API。

### 也可以看看

* class [Metered](../)
* 命名空间 [Aspose.Tasks](../../metered/)
* 部件 [Aspose.Tasks](../../../)


