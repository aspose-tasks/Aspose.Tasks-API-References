---
title: Interface IAlgorithmT
second_title: Справочник по Aspose.Tasks для .NET API
description: Aspose.Tasks.Util.IAlgorithm1T интерфейс. Представляет алгоритм который можно применить к списку объектовT .
type: docs
weight: 2390
url: /ru/net/aspose.tasks.util/ialgorithm-1/
---
## IAlgorithm&lt;T&gt; interface

Представляет алгоритм, который можно применить к списку объектов*T* .

```csharp
public interface IAlgorithm<in T>
```

| Параметр | Описание |
| --- | --- |
| T | Тип объекта, к которому применяется интерфейс метода. |

## Методы

| Имя | Описание |
| --- | --- |
| [Alg](../../aspose.tasks.util/ialgorithm-1/alg/)(T, int) | Обрабатывает объект в списке. Вызывается после[`PreAlg`](./prealg/) ; |
| [PostAlg](../../aspose.tasks.util/ialgorithm-1/postalg/)(T, int) | Вызывается после обработки объекта. |
| [PreAlg](../../aspose.tasks.util/ialgorithm-1/prealg/)(T, int) | Вызывается перед обработкой объекта. |

### Смотрите также

* пространство имен [Aspose.Tasks.Util](../../aspose.tasks.util/)
* сборка [Aspose.Tasks](../../)


