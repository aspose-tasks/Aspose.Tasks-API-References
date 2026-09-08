---
title: "Table.Equals"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Table 메서드. 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다"
type: docs
weight: 120
url: /ko/net/aspose.tasks/table/equals/
---
## Table.Equals method

이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다.

```csharp
public override bool Equals(object obj)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| obj | Object | 이 인스턴스와 비교할 객체. |

### 반환 값

**True** if the specified object is a Table that has the same UID value as this instance; otherwise, **false**.

## 예제

테이블 동등성을 확인하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Table> tables = project.Tables.ToList();

var table1 = tables[0];
var table2 = tables[1];

// 테이블의 동등성은 해당 테이블의 UID와 비교하여 확인됩니다.
Console.WriteLine("Table 1 UID: " + table1.Uid);
Console.WriteLine("Table 2 UID: " + table2.Uid);
Console.WriteLine("Are tables equal: " + table1.Equals(table2));
```

### 또 보기

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


