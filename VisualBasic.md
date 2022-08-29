## 12/08/22
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

## 16/08/2022
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
## 28/08/2022
Ejercicio utilizando case

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
## 29/08/2022
Crear registro

```
Sub guardar()
    fila = datos.Cells(1, 7)
    datos.Cells(fila, 1) = formulario.Cells(7, 4)
    datos.Cells(fila, 2) = formulario.Cells(9, 4)
    datos.Cells(fila, 3) = formulario.Cells(11, 4)
    datos.Cells(fila, 4) = formulario.Cells(13, 4)
    MsgBox ("los datos han sido guardados")
    datos.Cells(1, 7) = fila + 1
End Sub
```
