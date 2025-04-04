# Modernisering van legacy-systemen: onderhoud je IT-tuin

![De digitale tuin](./images/2025-04-03_digital-garden.png)

Je hoort het vaak: software is als het bouwen van een huis.
Maar die vergelijking gaat niet altijd op.
Een huis blijft jarenlang hetzelfde, terwijl software continu verandert.
Een tuin is daarom een betere metafoor.
In een tuin moet je regelmatig snoeien, bijmesten, onkruid verwijderen en rekening houden met het seizoen.
Hetzelfde geldt voor je IT-landschap.

Veel organisaties werken nog met verouderde software.
Deze legacy-systemen kampen met trage prestaties, kwetsbare beveiliging en onhandige afhankelijkheden van oude hardware of programmeertalen.
Modernisering is dan geen luxe, maar noodzaak.

## Waarom veranderen nodig is

Legacy klinkt negatief, maar is ook een erfenis: het systeem heeft het bedrijf jaren goed geholpen.
Maar dat succes uit het verleden biedt geen garantie voor de toekomst.
Als je niets verandert, ziet de komende vijf jaar er hetzelfde uit als de afgelopen vijf - en dat is zelden voldoende in de IT.

Technologische _en_ zakelijke veranderingen vragen om aanpassing.
Net als een tuin verschillende verzorging nodig heeft per seizoen, vraagt ook je softwareomgeving om flexibiliteit.
Denk aan de noodzaak tot opschalen, betere prestaties of het voldoen aan privacywetgeving.

In veel gevallen is bijscholing van mensen _en_ het vernieuwen van bestaande software goedkoper en efficiënter dan alles vanaf nul opnieuw opbouwen.
Maar als een systeem fundamenteel gebrekkig is, kan herbouw de enige oplossing zijn.

## Wat is een legacy-systeem?

We spreken van legacy als systemen gebouwd zijn in oudere talen als COBOL of C++, draaien op specifieke (vaak niet meer leverbare) hardware en moeilijk zijn te onderhouden.

Ook nieuwere systemen en software van 5-10 jaar oud, zoals .NET Framework, NodeJS of Java, kan als legacy gelden wanneer deze lastig te onderhouden of te integreren is.

Veelvoorkomende problemen zijn:

- Slechte prestaties en trage reacties
- Beveiligingslekken door oud geheugenbeheer
- Afhankelijkheid van oude infrastructuur
- Moeilijk te integreren met moderne systemen
- Hoge kosten en veel handmatige handelingen

## De kracht van moderne platforms

Bij ShareValue helpen we organisaties hun legacy-systemen te moderniseren, zonder dat alles overhoop hoeft.
Door te migreren naar moderne, platformonafhankelijke technologie (zoals .NET, Java, Docker, Kubernetes), creëer je meer flexibiliteit en schaalbaarheid.
Programmeertalen zoals Python, C# en JavaScript maken integraties makkelijker en de onderhoudbaarheid beter.

En ook belangrijk: veel organisaties gebruiken al moderne technologieën zoals Java naast oudere systemen als COBOL.
In die hybride situatie is goed systeemontwerp cruciaal.
Want technologie is maar één onderdeel van de oplossing; eenvoud en documentatie maken het verschil in onderhoudbaarheid.

## Grip op complexiteit

In moderne softwareomgevingen zie je vaak een web van onderlinge afhankelijkheden.
Tools zoals Terraform en Bicep helpen om infrastructuur via code te beheren.
Standaard-API's en cloudplatforms versnellen de ontwikkeling.
Maar hoe houd je overzicht in dit "digitale bos"?

Het antwoord ligt in observability: het meten en analyseren van prestaties, interacties en gedrag van systemen.
Door gebruik te maken van tools zoals JMeter, k6, Serilog, Application Insights of OpenTelemetry krijg je inzicht in:

- Reactietijden van API's
- Stabiliteit onder belasting (soak- en stresstests)
- Beveiligingslekken via simulatietesten
- Gebruikersgedrag en bottlenecks (met bijvoorbeeld Hotjar of Google Analytics)

Deze data helpt je om onderbouwde beslissingen te nemen en gericht te verbeteren.
Net als in een tuin weet je pas wat er nodig is als je eerst goed kijkt en meet.

## Kies voor veilige en onderhoudbare code

Moderne programmeertalen helpen je ook om beveiliging en onderhoudbaarheid structureel te verbeteren.
Denk aan:

- **C#** met nullable reference types (vanaf versie 8.0), die veelvoorkomende fouten zoals null reference exceptions voorkomen
- **Kotlin** met duidelijke syntax en integratie met Java, wat legacy-migraties vergemakkelijkt
- **Rust** dat geheugensveiligheid garandeert zonder garbage collector - ideaal voor gevoelige omgevingen zoals blockchain en IoT

Door moderne talen te gebruiken, voorkom je veel voorkomende bugs en verklein je het aanvalsoppervlak van je software.

```java
import java.util.Objects;

public class Person {
    private String name;
    private int age;

    public Person(String name, int age) {
        this.name = name;
        this.age = age;
    }

    public String getName() { return name; }
    public int getAge() { return age; }

    @Override
    public boolean equals(Object o) {
        if (this == o) return true;
        if (o == null || getClass() != o.getClass()) return false;
        Person person = (Person) o;
        // ❌ BUG: Missing comparison with the age 
        return Objects.equals(name, person.name);
    }

    @Override
    public int hashCode() {
        return Objects.hash(name, age);
    }

    @Override
    public String toString() {
        return "Person{name='" + name + "', age=" + age + "}";
    }
}
```

```java
import lombok.Data;

// ✅ Lombok's Data annotation causes the code to be generated
@Data
public class User {
    private String name;
    private int age;
}
```

```kotlin
// ✅ Kotlin's data class simplifies it even further
data class User(val name: String, val age: Int)
```

```csharp
using System;
using System.ComponentModel;
using System.Runtime.CompilerServices;

public class Person : INotifyPropertyChanged
{
    private string _name;
    private int _age;

    public event PropertyChangedEventHandler PropertyChanged;

    public string Name
    {
        get => _name;
        set
        {
            if (_name != value)
            {
                _name = value;
                // ⚠️ Newer developers may forget to call OnPropertyChanged
                OnPropertyChanged();
            }
        }
    }

    public int Age
    {
        get => _age;
        set
        {
            if (_age != value)
            {
                _age = value;
                OnPropertyChanged();
            }
        }
    }

    // ⚠️ This behavior could be repeated throughout the code
    protected virtual void OnPropertyChanged([CallerMemberName] string propertyName = "")
    {
        PropertyChanged?.Invoke(this, new PropertyChangedEventArgs(propertyName));
    }
}
```

```csharp
using CommunityToolkit.Mvvm.ComponentModel;

// ✅ MVVM Toolkit supports .NET Standard & provides base functionality
public partial class Person : ObservableObject
{
    // ✅ .NET source generators improve runtime performance
    [ObservableProperty] 
    private string _name;

    [ObservableProperty]
    private int _age;
}
```

```cpp
#include <iostream>

void badMemoryManagement() {
    int* ptr = new int(10);
    delete ptr; // Memory freed
    
    // ❌ BAD: Undefined behavior!
    std::cout << *ptr; // Accessing freed memory.
}

int main() {
    badMemoryManagement();
    return 0;
}
```

```rust
fn bad_memory_management() {
    let ptr = Box::new(10); // Heap allocation
    let reference = &*ptr;  // Borrow the value
    drop(ptr); // Move ownership out and drop the memory
    println!("{}", reference); // ❌ ERROR: Borrow after move
}

fn main() {
    bad_memory_management();
}
```

```shell
error[E0505]: cannot move out of `ptr` because it is borrowed
 --> src/main.rs:4:10
  |
2 |     let ptr = Box::new(10); // Heap allocation
  |         --- binding `ptr` declared here
3 |     let reference = &*ptr;  // Borrow the value
  |                     ----- borrow of `*ptr` occurs here
4 |     drop(ptr); // Move ownership out and drop the memory
  |          ^^^ move out of `ptr` occurs here
5 |     println!("{}", reference); // ❌ ERROR: Borrow after move
  |                    --------- borrow later used here
  |
help: consider cloning the value if the performance cost is acceptable
  |
3 -     let reference = &*ptr;  // Borrow the value
3 +     let reference = &ptr.clone();  // Borrow the value
  |

For more information about this error, try `rustc --explain E0505`.
error: could not compile `playground` (bin "playground") due to 1 previous error
```

```rust
fn safe_memory_management() {
    let data = vec![10]; // Owned by 'data'
    let ref_data = &data[0]; // Borrowed reference

    println!("{}", ref_data); // Safe access; cannot be used after data is freed
}

fn main() {
    safe_memory_management();
}
```

```javascript
function fetchData() {
    return new Promise((resolve) =>
        setTimeout(() => resolve("Data 1"), 1000)
    );
}

function fetchMoreData() {
    return new Promise((resolve) =>
        setTimeout(() => resolve("Data 2"), 1000)
    );
}

// ❌ BAD: Nested Promises create unnecessary sequential execution
fetchData().then(data1 => {
    console.log(data1);
    fetchMoreData().then(data2 => {
        // ❌ Nested promises are more difficult to understand
        console.log(data2);
    });
});
```

```javascript
const result = Promise.all([
    fetchData().then(data1 => console.log(data1)),
    fetchMoreData().then(data2 => console.log(data2))
]);

// ❌ This may print before promises resolve!
console.log("Finished processing!");
```


```typescript
// ✅ TypeScript's strong typing of results aids developers
async function fetchData(): Promise<string> {
    return new Promise(resolve =>
        setTimeout(() => resolve("Data 1"), 1000)
    );
}

async function fetchMoreData(): Promise<string> {
    return new Promise(resolve =>
        setTimeout(() => resolve("Data 2"), 1000)
    );
}

// ✅ async/await simplifies asynchronous logic & readability
async function fetchAllData() {
    
    const [data1, data2] = await Promise.all([
        fetchData(),
        fetchMoreData()
    ]);
    console.log(data1, data2);
    console.log("Finished processing!");
}

fetchAllData();
```


## Voorkom wildgroei

Softwarecode die je niet onderhoudt, groeit uit tot een verwilderde struik.
Tools zoals SonarQube, Checkstyle en CodeCharta helpen je om complexiteit inzichtelijk te maken.
Door cyclomatische complexiteit te meten of testcoverage te monitoren, houd je controle over de kwaliteit.

Let wel op: meer meten is niet altijd beter.
Wetmatigheden als Goodhart's Law, Amdahl's Law en Brooke's Law herinneren ons eraan dat je niet moet doorslaan.
Een goede balans tussen meten en verbeteren is essentieel.

## Documentatie als bodemlaag

Een goede tuin begint bij vruchtbare grond - en dat is in software je documentatie.
Zorg dat kennis over processen en systemen makkelijk vindbaar is.
Tools als Confluence of Markdown helpen daarbij.
Zelfs eenvoudige dingen als het meten van leestijd kunnen bijdragen aan betere betrokkenheid van lezers en gebruikers.

## ShareValue als jouw tuinman

Het moderniseren van legacy-systemen vraagt om kennis, ervaring en aandacht.
Bij ShareValue helpen we je graag om van een wildgroei aan systemen weer een beheerd en bloeiend IT-ecosysteem te maken.
Zodat jij je kunt focussen op je business, en met een gerust hart weet dat je IT klaar is voor de toekomst.

**Meer weten over legacy-modernisering** of sparren over je situatie? **Neem contact op met ShareValue** of lees onze andere blogs over cloudmigratie, observability of DevOps.
