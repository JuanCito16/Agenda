## Dia 12/08/22
Programacion en Visual Basic con el instructor Henry

```
Sub Sena ()
 nom = "luis"
 MsgBox nom
 num = 10
 MsgBox num
 nom = "maria"
 MsgBox "El nombre es: " & nom
End Sub
```

## Dia 16/08/2022
Ejercicio Visual Basic

```
Sub prueba()
    ing = InputBox("Ingresa su ingreso anual: ")
    
    If ing < 1000 Then
     MsgBox ("no hay impuesto")
    Else
        If ing >= 1001 And ing <= 10000 Then
            aum_imp = ing * 0.05
            MsgBox ("El total a pagar es: ") & aum_imp
        Else
            If ing >= 100001 And ing <= 1000000 Then
                aum_imp = ing * 0.15
                MsgBox ("El total a pagar es: ") & aum_imp
            Else
                If ing >= 1000001 And ing <= 10000000 Then
                    aum_imp = ing * 0.20
                    MsgBox ("El total a pagar es: ") & aum_imp
                Else
                    If ing > 10000001 Then
                    aum_imp = ing * 0.25
                    MsgBox ("El total a pagar es: ") & aum_imp
                    End If
                End If
            End If
        End If
    End If
End Sub
```
##28/08/2022

``` 
Sub caso()
    ing = InputBox("Ingresa su ingreso anual")
    Select Case ing
        Case 0 To 1000
            MsgBox ("No hay impuesto")
        Case 1001 To 10000
            aum_imp = ing * 0.05
            MsgBox ("El total a pagar es: ") & aum_imp
        Case 10001 To 100000
            aum_imp = ing * 0.15
            MsgBox ("El total a pagar es: ") & aum_imp
        Case 100001 To 10000000
            aum_imp = ing * 0.2
            MsgBox ("El total a pagar es: ") & aum_imp
        Case Else
            aum_imp = ing * 0.25
            MsgBox ("El total a pagar es: ") & aum_imp
    End Select
End Sub
``` 
