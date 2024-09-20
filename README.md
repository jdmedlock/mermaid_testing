# mermaid_testing
Test Mermaid Diagrams

```mermaid
  block-beta
    columns 5
    block:LEFT:2
      columns 1
      A1(("1"))
      space
      A2(("2"))
      space
      A3(("3"))
      space
      A6(("6"))
      space
      A7(("7"))
      space
      A8(("8"))
      space
      A10(("10"))
    end
    
    block:CENTER:1
      columns 1
      space
      SPRINT1("Sprint 1")
      space
      space
      space
      SPRINT2("Sprint 2")
      space
      space
      SPRINT35("Sprints 3-5")
      space
      space
      SPRINT6("Sprint 6")
    end
    
    block:RIGHT:2
      columns 1
      A4(("4"))
      space
      A5(("5"))
      space
      A9(("9"))
    end

    SPRINT1 --> SPRINT2
    SPRINT35 --> SPRINT6

    A1 -- "Meet team &</br>schedule Kickoff" --> SPRINT1
    A2 ----> SPRINT1
    A3 ----> SPRINT1
    A4 ----> SPRINT1
    A5 ----> SPRINT1
    A6 ----> SPRINT2
    A7 ----> SPRINT2
    A8 ----> SPRINT2
    A9 ----> SPRINT35
    A10 ----> SPRINT6
```