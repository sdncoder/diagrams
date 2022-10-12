### diagrams as code  

Mermaid diagramming:  
`https://mermaid-js.github.io/mermaid/#/`  
`https://www.freshbrewed.science/diagrams-as-code-mermaid/index.html`  

state diagram  
```
   stateDiagram
    direction LR  # set direction
    [*] --> main
    main --> branch
    branch --> review 
    review --> merge 
    merge --> main
```
```mermaid
   stateDiagram
   direction LR
    [*] --> main
    main --> branch
    branch --> review
    review --> merge
    merge --> main
 ```
 
 ```
  state branch {
    direction LR
    change --> review 
    review --> merge
    }
 ```
 ```mermaid
   stateDiagram
   direction LR
    [*] --> main
    main --> branch
    state branch {
    direction LR
    change --> review 
    review --> merge
    }
    merge --> main
 ```
 
 ```
 stateDiagram
   direction LR
    [*] --> main
    main --> branch : 1
    state branch {
    direction LR
    change --> review : 2
    review --> merge : 3
    }
    merge --> main : 4
    main --> ansible : 5
 ```

 ```mermaid
   stateDiagram
   direction LR
    [*] --> main
    main --> branch : 1
    state branch {
    direction LR
    change --> review : 2
    review --> merge : 3
    }
    merge --> main : 4
    main --> ansible : 5
 ```
 gitGraph
 
```mermaid
   gitgraph
        commit
        branch hotfix
        checkout hotfix
        commit
        branch develop
        checkout develop
```



