### diagrams

Mermaid diagramming  
`https://mermaid-js.github.io/mermaid/#/`  

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
    main --> ansible : git pull to Ansible repo
 ```
 