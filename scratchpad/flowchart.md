# ADRs, Idea Docs, RFCs, Design Docs, Oh My!

```mermaid
graph TD
A{Is there a problem?} -- No --> CELEB[Celebrate!]
A -- Yes --> SOLVED{Is there an existing or favored solution?}
SOLVED -- Yes --> DOC{Is it documented?}
DOC -- Yes --> CELEB
SOLVED -- No --> KNOWN{Do we know a solution?}
KNOWN -- No --> IDEA[Write an idea document]
IDEA --> TEST[Research or test ideas]
TEST --> BIG{Is it a big change?}
KNOWN -- Yes --> BIG
BIG -- No --> ADR[Write an ADR]
DOC -- No --> ADR
BIG -- Yes --> RFC[Write an RFC]
RFC --> K{Did the RFC result in a solution?}
K -- Yes --> L{Is it still a big change?}
L -- No --> ADR
L -- Yes --> DD[Write a design document]
```
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE1MzYxMzYwMjgsMzg3OTg3ODAxLDE4MT
Y3MjI2NzgsLTE2MTI3OTYxNjVdfQ==
-->