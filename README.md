# software-engineering

## Objektorientierung ##

- hilft die Komplexität in den Griff zu bekommen
- Objektorientierte Softwareentwicklung unterstützt dabei Software
  - einfacher erweiterbar,
  - besser testbar und
  - besser wartbar
zu machen

<details>
  <summary>Abstraktion</summary>

  - interne Implementierungsdetails verborgen
  -	nur „relevante“ Daten angezeigt

</details>

<details>
  <summary>Vererbung</summary>
  
  - Attribute und Methoden werden von einer Klasse zu einer anderen Klasse zur Verfügung gestellt 
  -	Zukünftige Anpassung müssen lediglich an einer Stelle durchgeführt werden
  - Code Wiederverwendung
</details>

<details>
  <summary>Kapselung</summary>
  
  - kontrollierter Zugriff auf Daten 
  -	erhöhte Datensicherheit
</details>

<details>
  <summary>Polymorphismus</summary>
  
  -	erlaubt Attribute und Methoden auszutauschen
</details>

## SOLID Prinzipien ##
- Objektorientierte Programmierung ist ein mächtiges Konzept
- führt jedoch nicht immer zu hochwertiger Software
- SOLID Prinzipien fokussieren sich auf dependency management
  - sofern sie berücksichtigt werden wird es einfacher
    - den Code zu pflegen (maintainable)
    - den Code wiederzuverwenden (reusable)
    - robusten Code zu erstellen
  - ansonsten wird Code spröde, fragil und schwer zu pflegen

### Single Responsibility ###
- 1 Klasse = 1 Responsibility
- die Klasse soll so klein wie möglich sein
- große Klassen sollen in kleinere Klassen aufgesplittet werden
- es sollte niemals mehr als einen Grund für eine Änderung geben

### Open/Close Principle ###
- Klassen sind _offen_ für Erweiterungen
- jedoch _geschlossen_ für Modifkationen
- private Varialben: getters und setters nur nutzen wenn sie benötigt werden
- benutze abstrakte Basisklassen wenn möglich

### Liskov Substitution Principle ###
- Objekte in einem Programm können durch Instanzen ihrer Subtypen ersetzt werden
- ohne die Korrektheit des Programms zu verändern
- verstöße scheitern häufig beim "ist ein"-Test
  - ein Quadrat "ist ein" Rechteck
  - jedoch ein Rechteck ist kein Quadrat
  
### Interface Segregation Principle ###
- großes Interface soll in fein abgestimmte Interfaces geteilt werden

### Dependency Inversion Principle ###
- Module höherer Ebenen sollten nicht von Modulen niedrigerer Ebenen abhängen
- Module sollten von Abstraktionen abhängen und Abstraktionen sollten nicht von Details abhängen
- Details sollten von Abstraktionen abhängen
