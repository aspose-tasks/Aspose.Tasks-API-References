---
title: "Aspose::Tasks::Metered クラス"
linktitle: "メータード"
articleTitle: "メータード"
second_title: "Aspose.Tasks for C++"
description: "メーターキーを設定するためのメソッドを提供します。"
type: docs
weight: 10
url: /ja/cpp/aspose.tasks/metered/
---

## Metered class

メーターキーを設定するためのメソッドを提供します。

この例では、メータードの公開鍵と秘密鍵を設定しようとします <ms>

```cpp
[C#]
 
Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");
 
 
[Visual Basic]
 
Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

</ms> <java> コンポーネントの jar ファイル:

```cpp
Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
```

</java>

## メソッド

| 名前 | 説明 |
| --- | --- |
| [GetConsumptionCredit](./getconsumptioncredit/) | 消費クレジットを取得します。 |
| [GetConsumptionQuantity](./getconsumptionquantity/) | 消費ファイルサイズを取得します。 |
| [IsLicensed](./islicensed/) | Metered ライセンスを使用して製品が正常にライセンスされているか確認します。 |
| [ResetMeteredKey](./resetmeteredkey/) | 以前に設定されたライセンスを削除します。 |
| [SetMeteredKey](./setmeteredkey/) | Metered の公開キーと秘密キーを設定します。 |

