<div align="center">

## Consequence Right\-Click


</div>

### Description

This is a code that someone by the name of Jared Collums had submitted. I took it and changed it so when someone right clicks on your web site it says "Please don't steal my source code.(Click again and something bad may happen." And the second time they right click your page instead of an unremovable messagebox popping up it just shuts down there web browser or if they are on AOL it closes AOL.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Mike](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/mike.md)
**Level**          |Intermediate
**User Rating**    |4.0 (20 globes from 5 users)
**Compatibility**  |
**Category**       |[Security](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/security__2-74.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/mike-consequence-right-click__2-1866/archive/master.zip)





### Source Code

```

  <SCRIPT LANGUAGE=JAVASCRIPT>
  document.onmousedown=click
  var times=0
  var times2=10
  function click() {
  if ((event.button==2) || (event.button==3)) {
  if (times>=1) { bye() }
  alert("Please don't steal my source code.(Click again and something bad may happen.");
  times++ } }
  function bye() {
  now = new Date()
var hours = now.getHours()
var minutes = now.getMinutes()
var seconds = now.getSeconds()
var ap = "AM"
 if (hours > 12)
   {var ap = "PM" , hours = hours-12 ;}
 if (minutes < 10)
   {minutes = "0"+minutes}
 if (seconds < 10)
   {seconds = "0"+seconds}
window.status = hours+":"+minutes+":"+seconds+" "+ap
document.title = hours+":"+minutes+":"+seconds+" "+ap
onload=bye()
  bye() }
  </SCRIPT>
```

