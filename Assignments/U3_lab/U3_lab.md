---
stylesheet: https://cdnjs.cloudflare.com/ajax/libs/github-markdown-css/2.10.0/github-markdown.min.css
body_class: markdown-body
css: |-
  .page-break { page-break-after: always; }
  .markdown-body { font-size: 14px; }
  .markdown-body pre > code { white-space: pre-wrap; }
pdf_options:
  margins : 25mm
  printBackground: true
---
# U3 Software Engineering lab 

## Team Details : 
- Name : P K Navin Shrinivas [PES2UG20CS237]
- Name : Mohamed Ayaan [PES2UG20CS200]
- Name : Mukund Deepak [PES2UG20CS206]
- Name : Nandan H [PES2UG20CS214]

## Problem 1B : 

## Problem 3 : 

- We have 4 contributors to the project, implying we have 4 branches + 1 main branch
![image](./3_1.png)

- Configuration Item table : 

| Item Name            | tracked? | Maintainer | Category    | Relation                    | Description                                                   |
|----------------------|----------|------------|-------------|-----------------------------|---------------------------------------------------------------|
| build.rs             | yes      | common     | build       | depends on proto            | Works as build script for software                            |
| main.rs              | yes      | common     | code        | driver code for all modules | Brings together entire program                                |
| data.proto           | yes      | Navin      | coupling    | build.rs depends on this    | Defines protocols for communication                           |
| .env                 | no       | common     | environment | -                           | Holds various build env vars                                  |
| target/              | no       | common     | build       | -                           | All builds go here                                            |
| CPUStat/lib.rs       | yes      | Navin      | code        | main.rs depends on this     | defines interface and modules for CPU module                  |
| CPUStat/statfuncs.rs | yes      | Navin      | code        | main.rs depends on this     | defines functions for CPU module                              |
| MEMStat/lib.rs       | yes      | Ayaan      | code        | main.rs depends on this     | defines interface and modules for MEM module                  |
| MEMStat/memfuncs.rs  | yes      | Ayaan      | code        | main.rs depends on this     | defines functions for MEM module                              |
| Cargo.toml           | yes      | common     | build       | build.rs depends on this    | Defines all modules and crate used for building this software |
|                      |          |            |             |                             |                                                               |

- Modifying Configuration Items | Ayaan : 
![image](./3_2.png)
![image](./3_3.png)
![image](./3_4.png)

- Modifying Configuration Items | Navin : 
![image](./3_5.png)
![image](./3_6.png)
![image](./3_7.png)





