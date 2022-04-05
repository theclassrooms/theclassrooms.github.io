# Structured Learning Path

The classroom is an attempt at community driven learning and guidance to all things software engineering, with ability to navigate into different levels of expertise based on an interest. This challenge

The aim is to cover learning paths to become a generalist or a specialist, but also enough of basic skills to be able to be an autonomous software engineer

The classroom contains guides, learning material, books, projects, documentation and other useful tips (cheatsheets, utility tooling, learning and productivity tooling)


> All square boxes are clickable to navigate through

<br />


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
            2 -.- 2c[basic programming with<br/> a language]
        end
        
        2 ------> 3[3 - Frontend Engineer]
        subgraph three
            3 -.- 3a[HTML and CSS]
            3 -.- 3b[Clean Code]
            3 -.- 3b[Design Patterns]
            3 -.- 3x[TBD]
        end
        subgraph four
            4 -.- 4a[core language]
            4 -.- 4b[Storage and databases]
            4 -.- 4c[Queueing]
            4 -.- 4d[Design Patterns]
            4 -.- 4e[Clean Code]
            4 -.- 4x[TBD]

        end

        2 ------> 4[4 - Backend Engineer]
        
        3 ------> 5
        3 --------> 6
        4 ------> 5[5 - Architecture and System Design]

        subgraph five
            5 -.- 5a[distributed systems <br/> distributed computing]
            5 -.- 5b[architecture patterns]
            5 -.- 5c[Scaling, availability,Consistency]
            5 -.- 5d[Databases and Caching design]
            5 -.- 5d[Networking and Security]
            5 -.- 5x[Event driven and Messaging]
        end
    

        4 ----------> 6[6 - Cloud Computing basics]

        subgraph six
            6 -.- 6a[Learning a Cloud]
            6 -.- 6b[TBD] 

        end
        
        6 ------> 7[7 - automation and operations]

        subgraph seven
            7 -.- 7a[CI/CD and devsecops]
            7 -.- 7b[Site Reliability] 

        end



        click 1 "./#/computer-science-fundamentals" "clickable"
        click 2 "./#/programming-fundamentals" "clickable"
        click 2b "./#/git" "clickable"

```

