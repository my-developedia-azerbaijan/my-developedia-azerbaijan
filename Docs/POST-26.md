![](../Img/oop.avif)

# Başlıq: OOP - Obyekt Yönlü Proqramlaşdırma nədir?

**Obyekt Yönlü Proqramlaşdırma (OOP) —** real dünyadakı obyektləri modelləşdirmək üçün istifadə olunan proqramlaşdırma yanaşmasıdır.
Sadə desək, kodu ardıcıl yazmaq əvəzinə, OOP kodu **siniflər (class)** və **obyektlər (object)** şəklində təşkil edir.

### OOP-un əsas prinsipləri:

OOP 4 əsas prinsipə əsaslanır. Bunlar aşağıdakılardır:

1. **Encapsulation (Kapsulyasiya):** Kapsulyasiya dəyişənləri və metodları (funksiyaları) bir sinif daxilində toplamaq və birbaşa çıxışı məhdudlaşdırmaqdır. 
    #### Niyə istifadə olunur?:
    - Məlumatları qoruyur,
    - Səhv dəyişikliklərin qarşısını alır,
    - Kod üzərində nəzarəti artırır
    #### Nümunə (Python):
    ```python
    class Student:
    def __init__(self, name):
        self.__name = name  # private (özəl/xüsusi) dəyişən

    def get_name(self):
        return self.__name
    ```
2. **Inheritance (İrsiyyət):** İrsiyyət, bir sinifin digər sinifdən xüsusiyyət və metodları miras almasıdır.
    #### Niyə istifadə olunur?:
    - Kod təkrarını azaldır, 
    - Daha səliqəli struktur yaradır
    #### Nümunə (Python):
    ```python
    class Animal:
    def speak(self):
        print("Heyvan səs çıxarır.")

    class Dog(Animal):
        def bark(self):
            print("İt hürür.")
        ```
3. **Polymorphism (Polimorfizm):** Polimorfizm, eyni metodun fərqli davranış göstərməsidir. 
    #### Nümunə (Python):
    ```python
    class Animal:
        def speak(self):
            print("Heyvan səsi")

    class Cat(Animal):
        def speak(self):
            print("Miyov")

    class Dog(Animal):
        def speak(self):
            print("Hav")
        ```
4. **Abstraction (Abstraksiya):** Abstraksiya, mürəkkəb detalları gizlədib yalnız əsas funksionallığı göstərməkdir.
    #### Niyə istifadə olunur?:
    - Mürəkkəbliyi azaldır,
    - "Necə işləyir" yox, "nə edir" fokuslanır
    #### Nümunə (Python):
    ```python
    from abc import ABC, abstractmethod

    class Vehicle(ABC):
        @abstractmethod
        def start(self):
            pass

    class Car(Vehicle):
        def start(self):
            print("Maşın açarla işə düşür")
        ```
### Sinif və Obyekt nədir?:

**Sinif (Class):** Obyekt yaratmaq üçün şablon (blueprint).
**Obyekt (Object):**  Sinifdən yaradılan konkret nümunə.

#### Nümunə (Python):
```python
class Car: #Car - Sinif (Class)
    def __init__(self, brand):
        self.brand = brand

car1 = Car("Mercedes-Benz") # Car("Mercedes-Benz") - Obyekt (Object)
car2 = Car("Land Rover") # Car("Land Rover") - Obyekt (Object)
```

### OOP-un üstünlükləri:

- ✅ Kodun təkrar istifadəsi,
- ✅ Daha asan baxım,
- ✅ Daha səliqəli struktur,
- ✅ Böyüyə bilən layihələr,
- ✅ Real dünya modelləşməsi

### OOP-un çatışmazlıqları:

- ❌ Daha mürəkkəbdir,
- ❌ Bir az daha yavaşdır,
- ❌ Dizayn düşüncəsi tələb edir
  
### OOP nə vaxt istifadə olunur?:

- Böyük layihələrdə,
- Layihədə tam idarə lazım olanda,
- Təmiz və oxunaqlı kod üçün,
- Real dünya modellərində

### Yekun:

OOP-un əsas ideyası:

1. Kodu obyektlərə bölmək,
2. Siniflərdən istifadə etmək,
3. 4 əsas prinsipə əməl etmək:
    - Kapsulyasiya
    - İrsiyyət
    - Polimorfizm
    - Abstraksiya

### Yekun tam sadə nümunə (Python):

```python
class BankAccount:
    def __init__(self, owner, balance):
        self.owner = owner
        self.balance = balance

    def deposit(self, amount):
        self.balance += amount

    def show_balance(self):
        print(self.balance)

account = BankAccount("Murad", 300)
account.deposit(150)
account.show_balance()
```

## Nəticə:

Obyekt yönlü proqramlaşdırma müasir proqram təminatının əsasını təşkil edən ən vacib yanaşmalardan biridir. Bu yanaşma proqramçıya kodu daha strukturlaşdırılmış, oxunaqlı və idarə oluna bilən formada yazmağa imkan verir. OOP-un əsas prinsipləri: **kapsulyasiya, irsiyyət, polimorfizm və abstraksiya**, proqramın həm təhlükəsizliyini, həm də genişlənə bilmə imkanlarını artırır. Bu prinsiplərdən düzgün istifadə edildikdə böyük və mürəkkəb layihələri daha rahat şəkildə idarə etmək mümkün olur. Həmçinin, OOP real dünya obyektlərini modelləşdirmək üçün çox effektiv bir üsuldur. Nəticə olaraq, OOP öyrənilməsi və tətbiqi hər bir proqramçı üçün vacib və faydalı bir bacarıqdır.



[**_by knvmrt_**](https://github.com/knvmrt)