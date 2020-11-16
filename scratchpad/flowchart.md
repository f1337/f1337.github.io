# ADRs, Idea Docs, RFCs, Design Docs, Oh My!

```mermaid
graph TD
PROBLEM{Is there a problem?} -- No --> CELEB[Celebrate!]
PROBLEM -- Yes --> ISSOLVED{Is there an existing or favored solution?}
ISSOLVED -- Yes --> DOC{Is it documented?}
DOC -- Yes --> CELEB
ISSOLVED -- No --> ISKNOWN{Do we know the solution?}
ISKNOWN -- No --> IDEA[Write an idea document]
IDEA --> TEST[Research or test ideas]
TEST --> ISKNOWN
ISKNOWN -- Yes --> ISBIG{Is it a big change?}
ISBIG -- No --> ADR[Write an ADR]
DOC -- No --> ADR
ISBIG -- Yes --> RFC[Write an RFC]
RFC --> RFCSOLVE{Did the RFC result in a solution?}
RFCSOLVE -- Yes --> ISBIGTOO{Is it still a big change?}
ISBIGTOO -- No --> ADR
ISBIGTOO -- Yes --> DD[Write a design document]
```
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE3Mzc5MDkzNTksMzg3OTg3ODAxLDE4MT
Y3MjI2NzgsLTE2MTI3OTYxNjVdfQ==
-->