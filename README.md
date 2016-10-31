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

<h1>Activity Dagram </h1>

```
@startuml
(*) --> "Login"
-->[You can sign out] "SignOut"
--> (*)
@enduml
```
<img src="https://github.com/Atcharee248/OOAD-WEEK11/blob/master/6.png?raw=true">


```
@startuml
(*) -up-> "wake"
-right-> "shower"
--> "gotoSchool"
-left-> (*)
@enduml
```
<img src="https://github.com/Atcharee248/OOAD-WEEK11/blob/master/7.png?raw=true">

```
@startuml
title Facebook
(*) --> "Login"

if "Password" then
  -->[true] "LoginSuccess"
  -right-> (*)
else
  ->[false] "LoginAgin"
  -->[WrongPassword] (*)
endif
@enduml
```
<img src="https://github.com/Atcharee248/OOAD-WEEK11/blob/master/8.png?raw=true">


```
@startuml
title RoBomyImagin
(*)  --> "check people"
If "Beautiful people" then
--> [Yes] "Request Line"
--> "walk through"
else
--> "walk through"
Endif
-->(*)
@enduml
```
<img src="https://github.com/Atcharee248/OOAD-WEEK11/blob/master/9.png?raw=true">

```
@startuml
(*) --> ===B1=== 
--> "home"
--> ===B2===

===B1=== --> "School"
--> ===B2===

--> (*)
@enduml
```
<img src="https://github.com/Atcharee248/OOAD-WEEK11/blob/master/10.png?raw=true">










