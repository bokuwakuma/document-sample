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
      A["デプロイ"] --> B{"本番環境か？"};
      B -- Yes --> C["不可"];
      B -- No --> D["デプロイコマンドの実行"];
      C ----> E["テスト"];
      D ----> E["テスト"];
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
