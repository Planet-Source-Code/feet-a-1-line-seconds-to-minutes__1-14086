<div align="center">

## A 1 Line Seconds To Minutes


</div>

### Description

This is a function to make seconds into minutes with just one line of code! It's completely commented and very easy to understand. I've seen some other one's that were like 20 or 30 linez long so i made this one. Very good for an mp3 player. I have more lines of comments than i do code :/
 
### More Info
 
you can have decimals at the end of your seconds like "126.33467" it would round that to "02:06" anything .5 or under round down, anything .5 or up rounds up.

It returns "00:00" in minutes then seconds like "02:52" after u put in 172.


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Feet](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/feet.md)
**Level**          |Beginner
**User Rating**    |3.3 (23 globes from 7 users)
**Compatibility**  |VB 4\.0 \(32\-bit\), VB 5\.0, VB 6\.0
**Category**       |[Math/ Dates](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/math-dates__1-37.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/feet-a-1-line-seconds-to-minutes__1-14086/archive/master.zip)

### API Declarations

u don't even have to dim anything!


### Source Code

```
Function SecsToMins(Secs As Integer)
If Secs < 60 Then SecsToMins = "00:" & Format(Secs, "00") Else SecsToMins = Format(Secs / 60, "00") & ":" & Format(Secs - Format(Secs / 60, "00") * 60, "00")
'if the seconds are less than 60 it will put a "00:" in front of it and the seconds formatted so if it was 6 seconds then it would be 06
'using format is pretty helpful
'if the seconds are 60 or are more than 60 it will
'divide the amount of seconds by 60 to get minutes
'then comes the harder to understand part(for some people)
'to get the seconds you have to format your seconds by 60 so there are no decimals. Then you multiple that by 60 and take that number away from the total seconds
'it took me awhile to figure out that i needed the format in the middle of finding the seconds.
End Function
```

