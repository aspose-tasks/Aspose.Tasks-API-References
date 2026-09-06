---
title: "LoadOptions.CancellationToken"
second_title: "Aspose.Tasks for .NET API 参考"
description: "LoadOptions 属性。获取或设置可用于取消项目加载操作的令牌。"
type: docs
weight: 20
url: /zh/net/aspose.tasks/loadoptions/cancellationtoken/
---
## LoadOptions.CancellationToken property

获取或设置可用于取消项目加载操作的令牌。

```csharp
public CancellationToken CancellationToken { get; set; }
```

## 示例

展示如何传递 CancellationToken 以取消长时间运行的项目加载操作。

```csharp
var loadOptions = new LoadOptions();

CancellationTokenSource cts = new CancellationTokenSource();
loadOptions.CancellationToken = cts.Token;

// cts 可以传递到另一个线程，在该线程中可以调用方法 cts.Cancel() 来取消项目加载操作。
// cts.Cancel();
var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);
```

### 另见

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


