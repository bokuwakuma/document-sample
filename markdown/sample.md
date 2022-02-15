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
  flowchart TEST;
      A[デプロイ] --> B{本番環境か？};
      B -- Yes --> C[不可];
      B -- No --> D[デプロイコマンドの実行];
      C ----> E[テスト];
      D ----> E[テスト];
```

### Graph

```mermaid
  graph TD;
      A-->B;
      A-->C;
      B-->D;
      C-->D;
```

