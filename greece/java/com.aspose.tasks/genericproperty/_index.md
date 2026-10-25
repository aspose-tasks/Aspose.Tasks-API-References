---
title: "GenericProperty"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά μια ιδιότητα δοχείου."
type: docs
weight: 113
url: /el/java/com.aspose.tasks/genericproperty/
---

**Inheritance:**
java.lang.Object
```
public class GenericProperty<TKey>
```

Αναπαριστά μια ιδιότητα δοχείου.

TKey : Ο τύπος της τιμής ιδιότητας.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [GenericProperty()](#GenericProperty--) | Αρχικοποιεί μια νέα παρουσία της κλάσης GenericProperty&lt;T&gt;. |
| [GenericProperty(Class&lt;TKey&gt; typeOfTKey, String name)](#GenericProperty-java.lang.Class-TKey--java.lang.String-) | Αρχικοποιεί μια νέα παρουσία της δομής GenericProperty&lt;TKey&gt;. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [&lt;TKey&gt;equals(GenericProperty&lt;TKey&gt; obj1, GenericProperty&lt;TKey&gt; obj2)](#-TKey-equals-com.aspose.tasks.GenericProperty-TKey--com.aspose.tasks.GenericProperty-TKey--) | Επιστρέφει μια τιμή που υποδεικνύει αν η καθορισμένη παρουσία `obj1` είναι ίση με την καθορισμένη παρουσία `obj2`. |
| [Clone()](#Clone--) | Δημιουργεί και επιστρέφει ένα βαθύ αντίγραφο αυτού του παραδείγματος. |
| [CloneTo(GenericProperty&lt;TKey&gt; that)](#CloneTo-com.aspose.tasks.GenericProperty-TKey--) | Δημιουργεί ένα βαθύ αντίγραφο της παρουσίασης σε άλλη παρουσίαση. |
| [clone()](#clone--) | \\{@inheritDoc\\} |
| [equals(Object obj)](#equals-java.lang.Object-) | \\{@inheritDoc\\} |
| [getName()](#getName--) | Λαμβάνει ένα όνομα της ιδιότητας. |
| [getValue()](#getValue--) | Λαμβάνει μια τιμή της ιδιότητας. |
### GenericProperty() {#GenericProperty--}
```
public GenericProperty()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης GenericProperty&lt;T&gt;.

### GenericProperty(Class&lt;TKey&gt; typeOfTKey, String name) {#GenericProperty-java.lang.Class-TKey--java.lang.String-}
```
public GenericProperty(Class<TKey> typeOfTKey, String name)
```


Αρχικοποιεί μια νέα παρουσία της δομής GenericProperty&lt;TKey&gt;.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| typeOfTKey | java.lang.Class&lt;TKey&gt; |  |
| name | java.lang.String | Το όνομα της ιδιότητας. |

### &lt;TKey&gt;equals(GenericProperty&lt;TKey&gt; obj1, GenericProperty&lt;TKey&gt; obj2) {#-TKey-equals-com.aspose.tasks.GenericProperty-TKey--com.aspose.tasks.GenericProperty-TKey--}
```
public static boolean <TKey>equals(GenericProperty<TKey> obj1, GenericProperty<TKey> obj2)
```


Επιστρέφει μια τιμή που υποδεικνύει αν η καθορισμένη παρουσία `obj1` είναι ίση με την καθορισμένη παρουσία `obj2`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| obj1 | [GenericProperty](../../com.aspose.tasks/genericproperty) | το πρώτο αντικείμενο για σύγκριση. |
| obj2 | [GenericProperty](../../com.aspose.tasks/genericproperty) | το δεύτερο αντικείμενο για σύγκριση. |

**Returns:**
boolean - επιστρέφει true εάν η καθορισμένη παρουσία `obj1` είναι ίση με την καθορισμένη παρουσία `obj2`; διαφορετικά, false.
### Clone() {#Clone--}
```
public GenericProperty<TKey> Clone()
```


Δημιουργεί και επιστρέφει ένα βαθύ αντίγραφο αυτού του παραδείγματος.

**Returns:**
[GenericProperty](../../com.aspose.tasks/genericproperty) - a deep copy of this object.
### CloneTo(GenericProperty&lt;TKey&gt; that) {#CloneTo-com.aspose.tasks.GenericProperty-TKey--}
```
public void CloneTo(GenericProperty<TKey> that)
```


Δημιουργεί ένα βαθύ αντίγραφο της παρουσίασης σε άλλη παρουσίαση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| that | [GenericProperty](../../com.aspose.tasks/genericproperty) | άλλη παρουσία. |

### clone() {#clone--}
```
public Object clone()
```




**Returns:**
java.lang.Object - \{@inheritDoc\}
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| obj | java.lang.Object | \\{@inheritDoc\\} |

**Returns:**
boolean - \{@inheritDoc\}
### getName() {#getName--}
```
public final String getName()
```


Λαμβάνει ένα όνομα της ιδιότητας.

**Returns:**
java.lang.String - ένα όνομα της ιδιότητας.
### getValue() {#getValue--}
```
public final Object getValue()
```


Λαμβάνει μια τιμή της ιδιότητας.

**Returns:**
java.lang.Object - μια τιμή της ιδιότητας.
