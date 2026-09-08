---
title: "Table.GetHashCode"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Table 메서드. 이 Table에 대한 해시 코드를 반환합니다"
type: docs
weight: 130
url: /ko/net/aspose.tasks/table/gethashcode/
---
## Table.GetHashCode method

이 테이블에 대한 해시 코드를 반환합니다.

```csharp
public override int GetHashCode()
```

### 반환 값

이 객체에 대한 해시 코드 값을 반환합니다.

## 예제

테이블의 해시 코드를 얻는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");

List<Table> tables = project.Tables.ToList();

var table1 = tables[0];
var table2 = tables[1];

// 테이블의 해시 코드는 테이블 UID와 같습니다.
Console.WriteLine("Table UID: {0} Hash Code: {1}", table1.Uid, table1.GetHashCode());
Console.WriteLine("Table UID: {0} Hash Code: {1}", table2.Uid, table2.GetHashCode());
```

### 또 보기

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


