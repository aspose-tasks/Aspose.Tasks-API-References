---
title: "CustomProjectPropertyCollection.Add"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "CustomProjectPropertyCollection yöntemi. Yeni bir özel property oluşturur"
type: docs
weight: 30
url: /tr/net/aspose.tasks.properties/customprojectpropertycollection/add/
---
## Add(string, string) {#add_3}

Yeni bir özel özellik oluşturur.

```csharp
public CustomProjectProperty Add(string name, string value)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | Dize | Özelliğin adı. |
| value | Dize | Yeni oluşturulan property nesnesinin değeri. |

### Dönüş Değeri

Yeni oluşturulan property nesnesi.

## Örnekler

Özel proje özelliği koleksiyonlarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

Console.WriteLine("Is custom properties collection read-only?: " + project.CustomProps.IsReadOnly);

// Yeni özel özellikler ekleyelim.
// Koleksiyon Boolean, DateTime, Double, String türlerini destekler.
project.CustomProps.Add("IsEnterprise", true);
project.CustomProps.Add("Project Start Date", new DateTime(2020, 4, 16, 8, 0, 0));
project.CustomProps.Add("Precision", 10d);
project.CustomProps.Add("Custom Name", "MyProject");

// Özel özellikler tiplenmiş koleksiyon aracılığıyla kullanılabilir.
Console.WriteLine("Count of custom properties: " + project.CustomProps.Count);
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
    Console.WriteLine();
}

// Bir özel özellik değerini al.
Console.WriteLine("Custom Name: " + project.CustomProps["Custom Name"]);

// Özel özelliklerin adları üzerinde yinele.
foreach (var propsName in project.CustomProps.Names)
{
    Console.WriteLine("Name: " + propsName);
    Console.WriteLine();
}

// Bir değer, string anahtar ile silinebilir.
if (project.CustomProps.Contains("Custom Name"))
{
    project.CustomProps.Remove("Custom Name");
}

// veya koleksiyonu tamamen temizleyebilir
project.CustomProps.Clear();
```

### Ayrıca Bakınız

* class [CustomProjectProperty](../../customprojectproperty/)
* class [CustomProjectPropertyCollection](../)
* namespace [Aspose.Tasks.Properties](../../customprojectpropertycollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string, bool) {#add}

Yeni bir özel özellik oluşturur.

```csharp
public CustomProjectProperty Add(string name, bool value)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | Dize | Özelliğin adı. |
| value | Boolean | Yeni oluşturulan property nesnesinin değeri. |

### Dönüş Değeri

Yeni oluşturulan property nesnesi.

## Örnekler

Özel proje özelliği koleksiyonlarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

Console.WriteLine("Is custom properties collection read-only?: " + project.CustomProps.IsReadOnly);

// Yeni özel özellikler ekleyelim.
// Koleksiyon Boolean, DateTime, Double, String türlerini destekler.
project.CustomProps.Add("IsEnterprise", true);
project.CustomProps.Add("Project Start Date", new DateTime(2020, 4, 16, 8, 0, 0));
project.CustomProps.Add("Precision", 10d);
project.CustomProps.Add("Custom Name", "MyProject");

// Özel özellikler tiplenmiş koleksiyon aracılığıyla kullanılabilir.
Console.WriteLine("Count of custom properties: " + project.CustomProps.Count);
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
    Console.WriteLine();
}

// Bir özel özellik değerini al.
Console.WriteLine("Custom Name: " + project.CustomProps["Custom Name"]);

// Özel özelliklerin adları üzerinde yinele.
foreach (var propsName in project.CustomProps.Names)
{
    Console.WriteLine("Name: " + propsName);
    Console.WriteLine();
}

// Bir değer, string anahtar ile silinebilir.
if (project.CustomProps.Contains("Custom Name"))
{
    project.CustomProps.Remove("Custom Name");
}

// veya koleksiyonu tamamen temizleyebilir
project.CustomProps.Clear();
```

### Ayrıca Bakınız

* class [CustomProjectProperty](../../customprojectproperty/)
* class [CustomProjectPropertyCollection](../)
* namespace [Aspose.Tasks.Properties](../../customprojectpropertycollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string, double) {#add_1}

Yeni bir özel özellik oluşturur.

```csharp
public CustomProjectProperty Add(string name, double value)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | Dize | Özelliğin adı. |
| value | Double | Yeni oluşturulan property nesnesinin değeri. |

### Dönüş Değeri

Yeni oluşturulan property nesnesi.

## Örnekler

Özel proje özelliği koleksiyonlarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

Console.WriteLine("Is custom properties collection read-only?: " + project.CustomProps.IsReadOnly);

// Yeni özel özellikler ekleyelim.
// Koleksiyon Boolean, DateTime, Double, String türlerini destekler.
project.CustomProps.Add("IsEnterprise", true);
project.CustomProps.Add("Project Start Date", new DateTime(2020, 4, 16, 8, 0, 0));
project.CustomProps.Add("Precision", 10d);
project.CustomProps.Add("Custom Name", "MyProject");

// Özel özellikler tiplenmiş koleksiyon aracılığıyla kullanılabilir.
Console.WriteLine("Count of custom properties: " + project.CustomProps.Count);
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
    Console.WriteLine();
}

// Bir özel özellik değerini al.
Console.WriteLine("Custom Name: " + project.CustomProps["Custom Name"]);

// Özel özelliklerin adları üzerinde yinele.
foreach (var propsName in project.CustomProps.Names)
{
    Console.WriteLine("Name: " + propsName);
    Console.WriteLine();
}

// Bir değer, string anahtar ile silinebilir.
if (project.CustomProps.Contains("Custom Name"))
{
    project.CustomProps.Remove("Custom Name");
}

// veya koleksiyonu tamamen temizleyebilir
project.CustomProps.Clear();
```

### Ayrıca Bakınız

* class [CustomProjectProperty](../../customprojectproperty/)
* class [CustomProjectPropertyCollection](../)
* namespace [Aspose.Tasks.Properties](../../customprojectpropertycollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string, DateTime) {#add_2}

Yeni bir özel özellik oluşturur.

```csharp
public CustomProjectProperty Add(string name, DateTime value)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | Dize | Özelliğin adı. |
| value | DateTime | Yeni oluşturulan property nesnesinin değeri. |

### Dönüş Değeri

Yeni oluşturulan property nesnesi.

## Örnekler

Özel proje özelliği koleksiyonlarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

Console.WriteLine("Is custom properties collection read-only?: " + project.CustomProps.IsReadOnly);

// Yeni özel özellikler ekleyelim.
// Koleksiyon Boolean, DateTime, Double, String türlerini destekler.
project.CustomProps.Add("IsEnterprise", true);
project.CustomProps.Add("Project Start Date", new DateTime(2020, 4, 16, 8, 0, 0));
project.CustomProps.Add("Precision", 10d);
project.CustomProps.Add("Custom Name", "MyProject");

// Özel özellikler tiplenmiş koleksiyon aracılığıyla kullanılabilir.
Console.WriteLine("Count of custom properties: " + project.CustomProps.Count);
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
    Console.WriteLine();
}

// Bir özel özellik değerini al.
Console.WriteLine("Custom Name: " + project.CustomProps["Custom Name"]);

// Özel özelliklerin adları üzerinde yinele.
foreach (var propsName in project.CustomProps.Names)
{
    Console.WriteLine("Name: " + propsName);
    Console.WriteLine();
}

// Bir değer, string anahtar ile silinebilir.
if (project.CustomProps.Contains("Custom Name"))
{
    project.CustomProps.Remove("Custom Name");
}

// veya koleksiyonu tamamen temizleyebilir
project.CustomProps.Clear();
```

### Ayrıca Bakınız

* class [CustomProjectProperty](../../customprojectproperty/)
* class [CustomProjectPropertyCollection](../)
* namespace [Aspose.Tasks.Properties](../../customprojectpropertycollection/)
* assembly [Aspose.Tasks](../../../)


