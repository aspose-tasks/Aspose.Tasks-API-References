---
title: "License.SetLicense"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод License. Лицензирует компонент."
type: docs
weight: 20
url: /ru/net/aspose.tasks/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

Лицензирует компонент.

```csharp
public void SetLicense(string licenseName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| licenseName | Строка | Может быть полным или коротким именем файла или именем встроенного ресурса. Используйте пустую строку, чтобы переключиться в режим оценки. |

## Примечания

Пытается найти лицензию в следующих местах:

1. Явный путь.

2. Папка, содержащая сборку компонента Aspose.

3. Папка, содержащая вызывающую сборку клиента.

4. Папка, содержащая входную (запускаемую) сборку.

5. Встроенный ресурс в вызывающей сборке клиента.

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. Явный путь.

2. Встроенный ресурс в вызывающей сборке клиента.

2. Папка, содержащая JAR‑файл компонента Aspose.

3. Папка, содержащая JAR‑файл, вызываемый клиентом.

## Примеры

В этом примере будет предпринята попытка найти файл лицензии с именем MyLicense.lic в папке, содержащей компонент, в папке, содержащей вызывающую сборку, в папке входной сборки, а затем во встроенных ресурсах вызывающей сборки.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");
```

файл jar компонента:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

Показывает, как применить лицензию Aspose.Tasks.

```csharp
var license = new License();
license.SetLicense("Aspose.Tasks.lic");
```

### См. также

* class [License](../)
* namespace [Aspose.Tasks](../../license/)
* assembly [Aspose.Tasks](../../../)

---

## SetLicense(Stream) {#setlicense}

Лицензирует компонент.

```csharp
public void SetLicense(Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Поток | Поток, содержащий лицензию. |

## Примечания

Используйте этот метод для загрузки лицензии из потока.

## Примеры

```csharp
[C#]

License license = new License();
license.SetLicense(myStream);


[Visual Basic]

Dim license as License = new License
license.SetLicense(myStream)

License license = new License();
license.setLicense(myStream);
```

Показано, как применить лицензию Aspose.Tasks, прочитанную из &lt;see cref="System.IO.FileStream" /&gt;.

```csharp
var license = new License();
using (var stream = new FileStream("Aspose.Tasks.lic", FileMode.Open))
{
    license.SetLicense(stream);
}
```

### См. также

* class [License](../)
* namespace [Aspose.Tasks](../../license/)
* assembly [Aspose.Tasks](../../../)


