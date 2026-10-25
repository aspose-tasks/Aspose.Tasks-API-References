---
title: "클래스 TableFieldCollection"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.TableFieldCollection 클래스. TableField 객체 목록을 포함합니다. IListTableField 인터페이스를 구현합니다."
type: docs
weight: 2350
url: /ko/net/aspose.tasks/tablefieldcollection/
---
## TableFieldCollection class

[`TableField`](../tablefield/) 객체 목록을 포함합니다. IList&lt;TableField&gt; 인터페이스를 구현합니다.

```csharp
public class TableFieldCollection : IList<TableField>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Count](../../aspose.tasks/tablefieldcollection/count/) { get; } | 이 컬렉션에 포함된 요소 수를 가져옵니다. |
| [IsReadOnly](../../aspose.tasks/tablefieldcollection/isreadonly/) { get; } | 이 컬렉션이 읽기 전용인지 여부를 나타내는 값을 가져옵니다; 그렇지 않으면 false. |
| [Item](../../aspose.tasks/tablefieldcollection/item/) { get; set; } | 지정된 인덱스에 있는 요소를 반환하거나 설정합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Add](../../aspose.tasks/tablefieldcollection/add/)(TableField) | 지정된 항목을 이 컬렉션에 추가합니다. |
| [Clear](../../aspose.tasks/tablefieldcollection/clear/)() | 이 컬렉션에서 모든 항목을 제거합니다. |
| [Contains](../../aspose.tasks/tablefieldcollection/contains/)(TableField) | 지정된 항목이 이 컬렉션에 있으면 true를 반환하고, 그렇지 않으면 false를 반환합니다. |
| [CopyTo](../../aspose.tasks/tablefieldcollection/copyto/)(TableField[], int) | 이 컬렉션의 요소를 지정된 배열에 복사하며, 지정된 배열 인덱스부터 시작합니다. |
| [GetEnumerator](../../aspose.tasks/tablefieldcollection/getenumerator/)() | 이 컬렉션에 대한 열거자를 반환합니다. |
| [IndexOf](../../aspose.tasks/tablefieldcollection/indexof/)(TableField) | 이 컬렉션에서 지정된 항목의 인덱스를 결정합니다. |
| [Insert](../../aspose.tasks/tablefieldcollection/insert/)(int, TableField) | 지정된 인덱스에 지정된 항목을 삽입합니다. |
| [Remove](../../aspose.tasks/tablefieldcollection/remove/)(TableField) | 이 컬렉션에서 특정 객체의 첫 번째 발생을 제거합니다. |
| [RemoveAt](../../aspose.tasks/tablefieldcollection/removeat/)(int) | 지정된 인덱스의 항목을 제거합니다. |

## 예제

테이블 필드 컬렉션을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project1.mpp");

foreach (var tbl in project.Tables)
{
    Console.WriteLine("Table name: " + tbl.Name);
    Console.WriteLine("Is collection of table fields read-only?: " + tbl.TableFields.IsReadOnly);

    // 테이블 필드를 반복합니다
    Console.WriteLine("Print table fields of " + project.Get(Prj.Name) + " project.");
    Console.WriteLine("Table count: " + tbl.TableFields.Count);
    foreach (var fld in tbl.TableFields)
    {
        Console.WriteLine("Field Title: " + fld.Title);
        Console.WriteLine("Field Field: " + fld.Field);
        Console.WriteLine();
    }
}

// 새 테이블 필드를 추가합니다
var table = project.Tables.ToList()[0];
var field = new TableField();
field.Title = "New Table Field";
table.TableFields.Add(field);

var field2 = new TableField();
field2.Title = "New Table Field 2";

// 해당 위치에 새 필드를 삽입합니다
var idx = table.TableFields.IndexOf(field);
table.TableFields.Insert(idx, field2);

// 인덱스 접근을 사용하여 새 테이블 필드를 편집합니다
table.TableFields[idx].WrapHeader = true;

Console.WriteLine("The collection contains the new table field?: " + table.TableFields.Contains(field));

// 최근에 필드를 제거할 수 있습니다
table.TableFields.RemoveAt(idx);

// 컬렉션을 두 가지 방법으로 정리할 수 있습니다
if (deleteOneByOne)
{
    // 테이블 필드를 배열에 복사하고 하나씩 삭제합니다
    var tableFields = new TableField[table.TableFields.Count];
    table.TableFields.CopyTo(tableFields, 0);
    foreach (var fld in tableFields)
    {
        table.TableFields.Remove(fld);
    }
}
else
{
    // 또는 테이블 필드 컬렉션을 완전히 비울 수 있습니다
    table.TableFields.Clear();
}
```

### 또 보기

* class [TableField](../tablefield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


