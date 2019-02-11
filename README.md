# Markdown ドキュメント

> このリポジトリは GitLab で管理し GitHub へミラーリングしています。

## 箇条書き

- A であること
- B であること

## 表

|            | 状況 |
| ---------- | ---- |
| GitLab     | o    |
| GitHub     | o    |
| VSCode MPE | o    |
| Typora     | o    |

| Left Aligned | Centered | Right Aligned | Left Aligned | Centered | Right Aligned |
| :----------- | :------: | ------------: | :----------- | :------: | ------------: |
| Cell 1       |  Cell 2  |        Cell 3 | Cell 4       |  Cell 5  |        Cell 6 |
| Cell 7       |  Cell 8  |        Cell 9 | Cell 10      | Cell 11  |       Cell 12 |

## 脚注

|            | 状況 |
| ---------- | ---- |
| GitLab     | o    |
| GitHub     | x    |
| VSCode MPE | o    |
| Typora     | △    |

この脚注は GitLab 用のもので、GitHub では動作しない。Typora ではポップアップ表示されるが脚注部分がそのままの位置に表示される。[^2]
[^2]: これは脚注です。

## details と summary

|            | 状況 |
| ---------- | ---- |
| GitLab     | o    |
| GitHub     | o    |
| VSCode MPE | o    |
| Typora     | x    |

<details>
<summary>この部分は GitLab、GitHub では展開/折りたたみ可能だがTyporaでは常に展開してしまう</summary>

These details _will_ remain **hidden** until expanded.

    PASTE LOGS HERE

</details>

## タスク

|            | 状況 |
| ---------- | ---- |
| GitLab     | o    |
| GitHub     | o    |
| VSCode MPE | o    |
| Typora     | o    |

- [x] Completed task
- [ ] Incomplete task
  - [ ] Sub-task 1
  - [x] Sub-task 2
  - [ ] Sub-task 3

## 図

### SVG

|            | 表示 |
| ---------- | ---- |
| GitLab     | x    |
| GitHub     | o    |
| VSCode MPE | o    |
| Typora     | o    |

#### yEd による SVG

![yEd](structure-yed.svg)

---

![yEd](structure.svg)

#### Pencil による SVG

![Pencil](structure-pencil.svg)

#### LibreOffice Draw による SVG

![LibreOffice Draw](structure-libreoffice-draw.svg)

#### OpenOffice Draw による SVG

![OpenOffice Draw](structure-openoffice-draw.svg)

### PNG

|            | 表示 |
| ---------- | ---- |
| GitLab     | o    |
| GitHub     | o    |
| VSCode MPE | o    |
| Typora     | o    |

#### yEd による PNG

![yEd](structure.png)

---

![yEd](git-branches.png)

---

![yEd](structure-yed.png)

#### Pencil による PNG

![Pencil](structure-pencil.png)

#### LibreOffice Draw による PNG

![LibreOffice Draw](structure-libreoffice-draw.png)

#### OpenOffice Draw による PNG

![OpenOffice Draw](structure-openoffice-draw.png)

## mermaid

|            | 図の表示 |
| ---------- | -------- |
| GitLab     | o        |
| GitHub     | x        |
| VSCode MPE | o        |
| Typora     | o        |

### シーケンス図

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

#### フローチャート

```mermaid
graph LR
    A[Hard edge] -->|Link text| B(Round edge)
    B --> C{Decision}
    C -->|One| D[Result one]
    C -->|Two| E[Result two]
```
