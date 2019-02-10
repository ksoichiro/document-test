# ヘッダ

## 構成

## 仕様

- A であること
- B であること

| 項目 | 説明 |
| ---- | ---- |
| a    | 1    |
| b    | 2    |

| Left Aligned | Centered | Right Aligned | Left Aligned | Centered | Right Aligned |
| :----------- | :------: | ------------: | :----------- | :------: | ------------: |
| Cell 1       |  Cell 2  |        Cell 3 | Cell 4       |  Cell 5  |        Cell 6 |
| Cell 7       |  Cell 8  |        Cell 9 | Cell 10      | Cell 11  |       Cell 12 |

You can add footnotes to your text as follows.[^2]
[^2]: This is my awesome footnote.

<details>
<summary>Click me to collapse/fold.</summary>

These details _will_ remain **hidden** until expanded.

    PASTE LOGS HERE

</details>

- [x] Completed task
- [ ] Incomplete task
  - [ ] Sub-task 1
  - [x] Sub-task 2
  - [ ] Sub-task 3

## 図

![draw.io](drawio.svg)

---

![yEd](structure-yed.svg)

---

![Pencil](structure-pencil.svg)

---

![LibreOffice Draw](structure-libreoffice-draw.svg)

---

![yEd](structure.svg)

## mermaid

```mermaid
sequenceDiagram
    Alice ->> Bob: Hello Bob, how are you?
    Bob-->>John: How about you John?
    Bob--x Alice: I am good thanks!
    Bob-x John: I am good thanks!
    Note right of John: Bob thinks a long<br/>long time, so long<br/>that the text does<br/>not fit on a row.

    Bob-->Alice: Checking with John...
    Alice->John: Yes... John, how are you?
```

---

```mermaid
sequenceDiagram
    participant Alice
    participant Bob
    Alice->>John: Hello John, how are you?
    loop Healthcheck
        John->>John: Fight against hypochondria
    end
    Note right of John: Rational thoughts<br/>prevail...
    John-->>Alice: Great!
    John->>Bob: How about you?
    Bob-->>John: Jolly good!
```

---

```mermaid
graph LR
    A[Hard edge] -->|Link text| B(Round edge)
    B --> C{Decision}
    C -->|One| D[Result one]
    C -->|Two| E[Result two]
```
