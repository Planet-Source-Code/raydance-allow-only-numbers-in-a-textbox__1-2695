<div align="center">

## Allow only numbers in a textbox\!


</div>

### Description

This program won't allow any other characters in a textbox then numbers and it allows you to use your Backspace key.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[RayDance](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/raydance.md)
**Level**          |Unknown
**User Rating**    |4.8 (24 globes from 5 users)
**Compatibility**  |VB 3\.0, VB 4\.0 \(16\-bit\), VB 4\.0 \(32\-bit\), VB 5\.0, VB 6\.0
**Category**       |[VB function enhancement](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/vb-function-enhancement__1-25.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/raydance-allow-only-numbers-in-a-textbox__1-2695/archive/master.zip)





### Source Code

```
Private Sub text1_KeyPress(KeyAscii As Integer)
  Dim Numbers As Integer
  Dim Msg As String
  Numbers = KeyAscii
  If ((Numbers < 48 Or Numbers > 57) And Numbers <> 8) Then
   Msg = MsgBox("Only Numbers are aloud in this Textbox", vbCritical, "Error Number")
   KeyAscii = 0
  End If
End Sub
```

