# OOAD-WEEK11
State Diagram

```
@startuml
[*] --> on
on --> [*]

on -> off
off -> on
off --> [*]
@enduml
```
<img src="https://github.com/Atcharee248/OOAD-WEEK11/blob/master/1.png?raw=true">


```
@startuml
[*] -> ready

ready : do/wait/for instruction
ready -> off : swich is turn off
off : do/shut down the power
off -> [*]
@enduml
```
<img src="https://github.com/Atcharee248/OOAD-WEEK11/blob/master/2.png?raw=true">


```
@startuml
[*] --> openThedoor
openThedoor --> closeThedoor

note left of openThedoor : walked home

note right of closeThedoor
 prevent bandit
end note
@enduml
```
<img src="https://github.com/Atcharee248/OOAD-WEEK11/blob/master/3.png?raw=true">


```
@startuml
title footballGame
[*] -> RMA
RMA : real madrid
RMA --> FCB : 1-0
RMA -> winner
FCB : barcelona
FCB -> Loser
winner -d->[*]
Loser -d-> [*]
FCB ->[*]
@enduml
```
<img src="https://github.com/Atcharee248/OOAD-WEEK11/blob/master/4.png?raw=true">


```
@startuml
[*] --> AlarmClock

state AlarmClock {
  state "Set the time" as Setthetime
  state "turn off" as turnoff
  [*] --> Setthetime
  Setthetime --> alarm : music
  alarm --> turnoff
  
}

AlarmClock --> [*]
@enduml
```
<img src="https://github.com/Atcharee248/OOAD-WEEK11/blob/master/5.png?raw=true">




