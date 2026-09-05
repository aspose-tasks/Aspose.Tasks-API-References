---
title: "ResourceValidationException"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "リソースプロパティでエラーが検出されたときにスローされる例外を表します。"
type: docs
weight: 260
url: /ja/java/com.aspose.tasks/resourcevalidationexception/
---

**Inheritance:**
java.lang.Object、java.lang.Throwable、java.lang.Exception、java.lang.RuntimeException、com.aspose.ms.System.Exception、com.aspose.ms.System.ApplicationException、[com.aspose.tasks.ValidationException](../../com.aspose.tasks/validationexception)
```
public class ResourceValidationException extends ValidationException
```

リソースのプロパティでエラーが見つかったときにスローされる例外を表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getResource()](#getResource--) | 例外の原因となったリソースを取得します。 |
### getResource() {#getResource--}
```
public final Resource getResource()
```


例外の原因となったリソースを取得します。

**Returns:**
[Resource](../../com.aspose.tasks/resource) - the resource which caused the exception.
