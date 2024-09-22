# mermaid_testing
Test Mermaid Diagrams

## Vertical Block Diagram

```mermaid
---
config:
  layout: elk
  theme: dark
---
  block-beta
    columns 9
    block:LEFT:4
      columns 1
      A1(("&nbsp;&nbsp;&nbsp; 1 &nbsp;&nbsp;&nbsp;"))
      A2(("&nbsp;&nbsp;&nbsp; 2 &nbsp;&nbsp;&nbsp;"))
      A3(("&nbsp;&nbsp;&nbsp; 3 &nbsp;&nbsp;&nbsp;"))
      A6(("&nbsp;&nbsp;&nbsp; 6 &nbsp;&nbsp;&nbsp;"))
      A8(("&nbsp;&nbsp;&nbsp; 8 &nbsp;&nbsp;&nbsp;"))
      A10(("&nbsp;&nbsp;&nbsp; 10 &nbsp;&nbsp;&nbsp;"))
    end
    
    block:CENTER:1
      columns 1
      space
      space
      space
      space
      SPRINT1("Sprint 1&nbsp;")
      space
      space
      space
      space
      space
      space
      space
      space
      SPRINT2("Sprint 2")
      space
      space
      space
      space
      SPRINT35("Sprints 3-5")
      space
      space
      SPRINT6("Sprint 6")
      space
    end
    
    block:RIGHT:4
      columns 1
      A4(("&nbsp;&nbsp;&nbsp; 4 &nbsp;&nbsp;&nbsp;"))
      A5(("&nbsp;&nbsp;&nbsp; 5 &nbsp;&nbsp;&nbsp;"))
      A7(("&nbsp;&nbsp;&nbsp; 7 &nbsp;&nbsp;&nbsp;"))
      A9(("&nbsp;&nbsp;&nbsp; 9 &nbsp;&nbsp;&nbsp;"))
    end

    SPRINT1 --> SPRINT2
    SPRINT2 --> SPRINT35
    SPRINT35 --> SPRINT6
    A1 -- "Meet team &</br>schedule Kickoff" --> SPRINT1
    A2 -- "Conduct Kickoff</br>Meeting" --> SPRINT1
    A3 -- "Update team list</br>in readme.md" --> SPRINT1
    A4 -- "Choose project &</br>define Vision stmt." --> SPRINT1
    A5 -- "Define & prioritize</br>features" --> SPRINT1
    A6 -- "Create Product</br>Backlog" --> SPRINT2
    A7 -- "Create wireframe" --> SPRINT2
    A8 -- "Setup team</br>workflow" --> SPRINT2
    A9 -- "Design, code,</br>test, & deploy app" --> SPRINT35
    A10 -- "Project Closure" --> SPRINT6

    style LEFT fill:#34495e
    style CENTER fill:#34495e
    style RIGHT fill:#34495e
    style A1 fill:#1d8348
    style A2 fill:#1d8348
    style A3 fill:#1d8348
    style A4 fill:#1d8348
    style A5 fill:#1d8348
    style A6 fill:#1d8348
    style A7 fill:#1d8348
    style A8 fill:#1d8348
    style A9 fill:#1d8348
    style A10 fill:#1d8348
    style SPRINT1 fill:#b9770e
    style SPRINT2 fill:#b9770e
    style SPRINT35 fill:#b9770e
    style SPRINT6 fill:#b9770e
```

## Horizontal Block Diagram

```mermaid
---
config:
  layout: elk
  theme: dark
---
  block-beta
    columns 4
    block:B1:1
      columns 1
      block:B1TOP
        columns 3
        A1(("&nbsp;&nbsp;&nbsp; 1 &nbsp;&nbsp;"))
        A2(("&nbsp;&nbsp;&nbsp; 2 &nbsp;&nbsp;"))
        A3(("&nbsp;&nbsp;&nbsp; 3 &nbsp;&nbsp;"))
      end
      space
      space
      block:B1CENTER
        columns 3
        space
        SPRINT1("&nbsp;Sprint 1&nbsp;")
        space
      end
      space
      space
      block:B1BOTTOM
        columns 3
        A4(("&nbsp;&nbsp;&nbsp; 4 &nbsp;&nbsp;"))
        space
        A5(("&nbsp;&nbsp;&nbsp; 5 &nbsp;&nbsp;"))
      end
      A1 -- "Meet team &</br>schedule</br>Kickoff" --> SPRINT1
      A2 -- "</br></br></br></br></br></br>Hold</br>Kickoff" --> SPRINT1
      A3 -- "Update</br>readme.md</br>team list" --> SPRINT1
      A4 -- "Choose</br>project &</br>define</br>vision stmt." --> SPRINT1
      A5 -- "Define &</br>prioritize</br>features" --> SPRINT1
    end

    block:B2:1
      columns 1
      block:B2TOP
        columns 3
        A6(("&nbsp;&nbsp;&nbsp; 6 &nbsp;&nbsp;"))
        space
        A7(("&nbsp;&nbsp;&nbsp; 7 &nbsp;&nbsp;"))
      end
      space
      space
      block:B2CENTER
        columns 3
        space
        SPRINT2("&nbsp;Sprint 2&nbsp;")
        space
      end
      space
      space
      block:B2BOTTOM
        columns 3
        space
        A8(("&nbsp;&nbsp;&nbsp; 8 &nbsp;&nbsp;"))
        space
      end
      A6 -- "Create</br>Product</br>Backlog" --> SPRINT2
      A7 -- "Create</br>Wireframe" --> SPRINT2
      A8 -- "Define team workflow" --> SPRINT2
    end

    block:B3:1
      columns 1
      block:B3TOP
        columns 3
        space
        A9(("&nbsp;&nbsp;&nbsp; 9 &nbsp;&nbsp;"))
        space
      end
      space
      space
      space
      space
      block:B3CENTER
        columns 3
        space
        SPRINTS35("&nbsp;Sprint 3-5 ")
        space
      end
      space
      block:B3BOTTOM
        columns 3
        space
        space
        space
      end
      A9 -- "Design, code,</br>test & deploy" --> SPRINTS35
    end

    block:B4:1
      columns 1
      block:B4TOP
        columns 3
        space
        A10(("&nbsp;&nbsp;&nbsp;10&nbsp;"))
        space
      end
      space
      space
      block:B4CENTER
        columns 3
        space
        SPRINT6("&nbsp;Sprint 6&nbsp;")
        space
      end
      space
      space
      block:B4BOTTOM
        columns 3
        space
        space
        space
      end
      A10 -- "Project Closure" --> SPRINT6
    end

    SPRINT1 --> SPRINT2
    SPRINT2 --> SPRINTS35
    SPRINTS35 --> SPRINT6

    style B1TOP stroke:#292d30,fill:#292d30

    style A1 fill:#1d8348
    style A2 fill:#1d8348
    style A3 fill:#1d8348
    style A4 fill:#1d8348
    style A5 fill:#1d8348
    style A6 fill:#1d8348
    style A7 fill:#1d8348
    style A8 fill:#1d8348
    style A9 fill:#1d8348
    style A10 fill:#1d8348
    style SPRINT1 fill:#b9770e
    style SPRINT2 fill:#b9770e
    style SPRINTS35 fill:#b9770e
    style SPRINT6 fill:#b9770e
```
