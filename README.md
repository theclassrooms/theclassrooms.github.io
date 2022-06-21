# Structured Learning Path

[![theclassroom](https://img.shields.io/badge/theclassroom-dev-blue)](https://theclassroom.dev) is an attempt at community-driven learning and guidance to all things software engineering, with the ability to navigate into different levels of expertise based on interest. This challenge

The aim is to cover learning paths to becoming a generalist or a specialist, but also enough basic skills to be able to be an autonomous software engineer

The classroom contains guides, learning material, books, projects, documentation, and other valuable tips (cheatsheets, utility tooling, learning, and productivity tooling). The following is a flow of direction represented using [mermaid](https://mermaid-js.github.io/mermaid/#/) for the learning path

> All rectangle boxes are clickable to dive into that area in the following figure.

```mermaid
graph TD

        0{level 0} -->|Start her for <br/> 0 tech experience| 1

        1[1 - Computer Science fundamentals] ------> 2[2 - Programming fundamentals]
        subgraph one
            1 -.- 1a[computer architecture]
            1 -.- 1b[operating systems]
            1 -.- 1c[linux and shell]
        end

        subgraph two
            2 -.- 2a[algorithms and datastructures]
            2 -.- 2b[git and github]
            2 -.- 2c[basics of programming]
        end

        2 ------> 3a[3a - Frontend Engineer]
        subgraph three-A
            3a -.- 3aa[HTML and CSS]
            3a -.- 3ab[Clean Code]
            3a -.- 3ac[Design Patterns]
            3a -.- 3ax[TBD]
        end

        2 ------> 3b[3b - Backend Engineer]
        subgraph three-B
            3b -.- 3ba[core language]
            3b -.- 3bb[Storage and databases]
            3b -.- 3bc[Queueing]
            3b -.- 3bd[Design Patterns]
            3b -.- 3be[Clean Code]
            3b -.- 3bx[TBD]

        end


        3a ------> 4
        3b ------> 4[4 - Architecture and System Design]

        subgraph four
            4 -.- 4a[distributed systems <br/> distributed computing]
            4 -.- 4b[architecture patterns]
            4 -.- 4c[Scaling, availability,Consistency]
            4 -.- 4d[Databases and Caching design]
            4 -.- 4d[Networking and Security]
            4 -.- 4x[Event driven and Messaging]
        end

        3a ----------> 5
        3b ----------> 5[5 - Cloud Computing basics]

        subgraph five
            5 -.- 5a[LearnCloud]
            5 -.- 5b[IaC]
        end

        5 ------> 6[6 - automation and operations]

        subgraph six
            6 -.- 6a[CI/CD and devsecops]
            6 -.- 6b[Site Reliability]

        end



        click 1 "./#/computer-science-fundamentals" "x"
        click 1a "./#/computer-architecture" "x"
        click 1b "./#/operating-systems" "x"
        click 1c "./#/linux-and-shell" "x"
        click 2 "./#/programming-fundamentals" "x"
        click 2b "./#/git" "x"
        click 2a "./#/algorithms-and-data-structures" "x"
        click 2c "./#/basics-of-programming" "x"
        click 5a "./#/learning-a-cloud" "x"
        click 5b "./#/iac" "x"

```
