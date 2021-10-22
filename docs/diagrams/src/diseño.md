**Problema**. No se desea que *Supermarket* se complique con cada uno de los menús y tickets de cada país. 

* Programar para la interfaz, no para la implementación: *Abstract Factory*

**Intención**. Provee una interfaz para crear familias de objetos 
relacionados o dependientes sin especificar sus clases 
concretas

**Interrelación**. Singleton, Factory Method y Prototype

**Propósito**. 

* ~Abstract Factory vs Facade~. No se trata de ocultar un subsistema 
 …

* ~Abstract Factory vs Builder~. No se trata de una creación compleja
 …

**Rediseño**. Creando un objeto especificando una clase explícitamente (*SpanishMenu y FrenchMenu*)

**Variación**. Familias de objetos “producto” (derivadas de *Menu*)

![abstractFactory](../out/abstractFactory.svg)


**Problema**. No se desea complicar los algoritmos del Menú con la particularidad de cada país. 

* Determinando la granularidad de los objetos : **Command**

**Intención**. Encapsula una petición como un objeto, permitiendo de ese modo parametrizar clientes con 
diferentes peticiones, colas o solicitudes registradas, y apoyar las operaciones de deshacer.

**Interrelación**. *Prototype, ~Memento y Composite~*

**Propósito**. 

* *~Command vs Memento.~* No se trata de recuperar estados anteriores …

**Rediseño**. Dependencias de operaciones algorítmicas: podrá haber nuevas opciones

**Variación**. Cómo y cuándo una operación es gestionada

![Command](../out/Command.svg)

**Problema**. No se desea complicar los algoritmos del *Menú* con la particularidad de cada país. 

* Programando para la interfaz, no para la implementación: 
*Template Method*

**Intención**. Define el esqueleto de un algoritmo en una operación difiriendo algunos pasos a las subclases que redefinen esos pasos del algoritmo sin cambiar la estructura

**Interrelación**. 

**Propósito.** 
* ~Template Methos vs Strategy~. No se requiere dinamismo …

**Rediseño**. Dependencias algorítmicas de la configuración del menú por país

**Variación**. Pasos de un algoritmo

![templateMethod](../out/templateMethod.svg)


**Problema**. No se desea complicar los algoritmos del *Ticket* con la particularidad de cada país. 

* Determinando la granularidad de los objetos : **Visitor**

**Intención**. Representa una operación para ser realizadas sobre los elementos de una estructura de objetos y permite 
definir nuevas operaciones sin cambiar las clases de elementos sobre los que opera

**Interrelación**. 

**Propósito**. 

**Rediseño**. Inhabilidad para cambiar una clase adecuadamente: podrá haber nuevas operaciones

**Variación**. Operaciones que pueden ser aplicadas a objetos sin cambiar su clase


**Problema**. No se desea complicar al *Ticket* con la particularidad del número de operaciones. 

* Relacionando tiempo de compilación vs ejecución: **Composite**

**Intención**. Compone objetos en estructuras arbóreas para representar las jerarquía de todo-parte y permite a los clientes 
tratar con objetos individuales y objetos compuestos uniformemente

**Interrelación**. *Iterator, Visitor, Chain of Responsability*, …

**Propósito**. 

* ~Composite vs Decorator~: No se pretende aportar funcionalidades dinámicamente …

**Rediseño**. Relacionando tiempo de compilación y de ejecución

**Variación**. La estructura y composición de un objeto


**Problema**. No se desea complicar los algoritmos del *Ticket* con la particularidad de cada país. 

* Delegación: **Strategy**

**Intención**. Define una familia de algoritmos, encapsula cada uno y los hace intercambiables. Permite al algoritmo variar 
independientemente del cliente que lo use

**Interrelación**. *Flyweight*

**Propósito**. 
* ~Strategy vs Decorator~. No interesa aportar nueva funcionalidad …

* ~Strategy vs Template Method~. Aumenta número de clases …

**Rediseño**. Dependencias algorítmicas

**Variación**. Un algoritmo

![visitorComposite](../out/visitorComposite.svg)

**Problema**. No se desea complicar los algoritmos del *Ticket* con la particularidad de cada país. 

* Programando para la interfaz, no para la implementación: 
**Builder**

**Intención**. Separa la construcción de un objeto complejo de 
su representación de tal forma que el mismo proceso de construcción puede crear diferentes representaciones

**Interrelación**. *Singleton, Composite, Abstract Factory/Prototype*

**Propósito**. 

**Rediseño**. Dependencias algorítmicas

**Variación**. Cómo se crea un compuesto

![builder](../out/builder.svg)

**Visión general de clases principales**

![overview](../out/overview.svg)

**Arquitectura del software (jerarquía de paquetes)**

![v5](../diagrams/out/v5.svg)
