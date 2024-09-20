# mermaid_testing
Test Mermaid Diagrams

```mermaid
  block-beta
    columns 9
    block:LEFT:4
      columns 1
      A1(("&nbsp;&nbsp; 1 &nbsp;&nbsp;"))
      A2(("&nbsp;&nbsp; 2 &nbsp;&nbsp;"))
      A3(("&nbsp;&nbsp; 3 &nbsp;&nbsp;"))
      A6(("&nbsp;&nbsp; 6 &nbsp;&nbsp;"))
      A8(("&nbsp;&nbsp; 8 &nbsp;&nbsp;"))
      A10(("&nbsp;&nbsp; 10 &nbsp;&nbsp;"))
    end
    
    block:CENTER:1
      columns 1
      space
      space
      space
      space
      space
      SPRINT1("&nbsp;&nbsp;Sprint 1&nbsp;&nbsp;")
      space
      space
      space
      space
      space
      space
      SPRINT2("&nbsp;Sprint 2&nbsp;")
      space
      space
      space
      space
      SPRINT35("&nbsp;Sprints 3-5&nbsp;")
      space
      space
      SPRINT6("&nbsp;Sprint 6&nbsp;")
      space
    end
    
    block:RIGHT:4
      columns 1
      A4(("&nbsp;&nbsp; 4 &nbsp;&nbsp;"))
      A5(("&nbsp;&nbsp; 5 &nbsp;&nbsp;"))
      A7(("&nbsp;&nbsp; 7 &nbsp;&nbsp;"))
      A9(("&nbsp;&nbsp; 9 &nbsp;&nbsp;"))
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

```