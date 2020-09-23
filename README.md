<div align="center">

## Randomize


</div>

### Description

Ensure that the random number generator is seeded properly.
 
### More Info
 
Using the VB statement "Randomize" by itself to seed the random number generator implicitly means "Randomize Timer", with the timer function returning the number of seconds that have elapsed since 12:00 A.M. (midnight). If a program is started at roughly, or worse, launched at the same time each day, the timer could return the same seed each day. To avoid this problem, use a seed based on the date and time.


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Tom Rezek](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/tom-rezek.md)
**Level**          |Unknown
**User Rating**    |5.0 (10 globes from 2 users)
**Compatibility**  |VB 3\.0, VB 4\.0 \(16\-bit\), VB 4\.0 \(32\-bit\), VB 5\.0, VB 6\.0
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__1-1.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/tom-rezek-randomize__1-860/archive/master.zip)

### API Declarations

none


### Source Code

```

' Ensure a random seed even if the program is started at exactly the same time each day.
Randomize Int(CDbl((Now))) + Timer
```

