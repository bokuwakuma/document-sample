# Markdown Sample

## With Mermaid

### Java

```java
Class Sample {
    private String test;
    private String test1;

    public setTest(String test) {
        this.test = test;
    }

    public getTest() {
        return test;
    }
}
```

### Flowchart

```mermaid
  flowchart TD
      A[deploy phase] --> B{production?};
      B -- Yes --> C[not deploy];
      B -- No --> D[run deploy command.];
      C ----> E[test phase];
      D ----> E[test phase];
```

```mermaid
flowchart TD
    A[Start] --> B{Is it?};
    B -->|Yes| C[OK];
    C --> D[Rethink];
    D --> B;
    B ---->|No| E[End];
```

### Graph

```mermaid
  graph TD;
      A-->B;
      A-->C;
      B-->D;
      C-->D;
```

### Class Diagram

```mermaid
 classDiagram
      Animal <|-- Duck
      Animal <|-- Fish
      Animal <|-- Zebra
      Animal : +int age
      Animal : +String gender
      Animal: +isMammal()
      Animal: +mate()
      class Duck{
          +String beakColor
          +swim()
          +quack()
      }
      class Fish{
          -int sizeInFeet
          -canEat()
      }
      class Zebra{
          +bool is_wild
          +run()
      }
```
