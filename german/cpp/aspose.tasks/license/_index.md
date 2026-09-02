---
title: "Aspose::Tasks::License Klasse"
linktitle: "License"
articleTitle: "License"
second_title: "Aspose.Tasks für C++"
description: "Stellt Methoden zur Lizenzierung der Komponente bereit."
type: docs
weight: 10
url: /de/cpp/aspose.tasks/license/
---

## License class

Stellt Methoden zur Lizenzierung der Komponente bereit.

In diesem Beispiel wird versucht, eine Lizenzdatei mit dem Namen MyLicense.lic im Ordner zu finden, der <ms> die Komponente enthält, im Ordner, der die aufrufende Assembly enthält, im Ordner der Einstieg‑Assembly und anschließend in den eingebetteten Ressourcen der aufrufenden Assembly.

```cpp
[C#]
 
License license = new License();
license.SetLicense("MyLicense.lic");
 
 
[Visual Basic]
 
Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

</ms> <java> die Komponenten-JAR-Datei:

```cpp
License license = new License();
license.setLicense("MyLicense.lic");
```

</java>

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [License](./license/) | Initialisiert eine neue Instanz der License‑Klasse. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [SetLicense (2 overloads)](./setlicense/) | Lizenziert die Komponente. |

