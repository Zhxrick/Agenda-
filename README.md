
### Programacion general 
´´´´


Sub sena

nom = "julissa" 
num = "10" 
nom = "zharick" 

end Sena

´´´´
### FECHA: 19/08/2022

Sub Suma()
 a = Int(InputBox("digitar numero para la variable a"))
 b = Int(InputBox("Digitar numero para la variable b"))
 
 c = a + b
 
 MsgBox "El resultado es:" & c


End Sub


### Descuento numero de noche

definir noche, precio, pago como entero
	definir descuento como real
	
	precio<- 100
	escribir "Digite el numero de noches"
	leer noches
	
	total <- precio * noches
	
	si noches > 3 entonces 
		descuento <- total*.05
		
		 escribir "Su pago total es: ", total - descuento 
	sino 
		
		escribir "su pago total sin descuento es: ", total
		
		
	FinSi

### Sacar promedio de notas / aprobado no aprobado 
Algoritmo sin_titulo
	
	definir alumno como caracter 
	definir examenparcial, examenfinal,promediopracticas como real
	definir final Como Real
	
	escribir "Digite el nombre del alumno" 
	leer alumno 
	
	Escribir "Las notas se calificaran de 1 - 10" 
	
	Escribir "Digite la nota del examen parcial"
	leer examenparcial
	Escribir "Digite la nota del examen final"
	leer examenfinal
	Escribir "Digite la nota del promedio de practicas"
	leer promediopracticas
	
	final <- (examenparcial+promediopracticas+(examenfinal*2))/3
	
	si final > 6 entonces 
		escribir "alumno aprobado: ", alumno 
		escribir "su promedio es: ", final 
	sino 
		
		escribir alumno, " alumno no aprobado"
		escribir "su promedio es: ", final 
		
	FinSi
	
FinAlgoritmo


### Impuesto anual de una empresa usando If - Else

Sub sena()

    ingreso_anual = InputBox("Digite los ingresos anuales de la empresa: ")
    Total = 0
    impuesto = 0
    aumento = 0
    
    If ingreso_anual < 1000 And ingreso_anual > 0 Then
      MsgBox ("No debe pagar impuestos")
    Else
        If ingreso_anual >= 1001 And ingreso_anual <= 10000 Then
            aumento = (ingreso_anual * 0.05)
            MsgBox ("Total impuesto a pagar: ") & aumento
        Else
            If ingreso_anual >= 10001 And ingreso_anual <= 100000 Then
            aumento = (ingreso_anual * 0.1)
            MsgBox ("Total impuesto a pagar: ") & aumento
            
            Else
                If ingreso_anual >= 100001 And ingreso_anual <= 1000000 Then
                    aumento = (ingreso_anual * 0.15)
                    MsgBox ("Total impuesto a pagar: ") & aumento
                Else
                      If ingreso_anual >= 100000 And ingreso_anual <= 10000000 Then
                         aumento = (ingreso_anual * 0.2)
                          MsgBox ("Total impuesto a pagar: ") & aumento
                      Else
                           If ingreso_anual >= 10000001 Then
                                aumento = (ingreso_anual * 0.25)
                                MsgBox ("Total impuesto a pagar: ") & aumento
                            Else
                                MsgBox "No se puede calcular"
                           End If
                          
                      End If
                
                End If
                
            End If
                    
        End If

    End If

End Sub
 
 ### Impuesto anual de una empresa usando Case 
 
 Sub sena()

      ingreso_anual = Int(InputBox("Digite los ingresos anuales de la empresa: "))
      aumento = 0
      
      Select Case ingreso_anual
      
      Case 0 To 1000
      MsgBox ("No debe pagar impuestos")
      
      Case 1001 To 10000
      aumento = (ingreso_anual * 0.05)
      MsgBox ("El total de impuestos a pagar es: ") & aumento
      
      Case 10001 To 100000
      aumento = (ingreso_anual * 0.1)
      MsgBox ("El total de impuesto a pagar es: ") & aumento
      
      Case 100001 To 1000000
      aumento = (ingreso_anual * 0.15)
      MsgBox ("El total de impuestos a pagar es: ") & aumento
      
      Case 1000000 To 10000001
      aumento = (ingreso_anual * 0.2)
      MsgBox ("El total de impuestos a pagar es: ") & aumento
      
      End Select
      
      If ingreso_anual >= 10000001 Then
                            aumento = (ingreso_anual * 0.25)
                            MsgBox ("Total impuesto a pagar: ") & aumento
                            
      End If

End Sub

	
### Hacer un formulario

Private Sub CommandButton1_Click()

End Sub

Private Sub btnguardar_Click()

Dim llenar As Long
 Sheets("DATOS").Activate

 llenar = WorksheetFunction.CountA(Range("A:A")) + 1
  
   Cells(llenar, 1).Value = Textnombre.Value
   Cells(llenar, 2).Value = Textapellido.Value
   Cells(llenar, 4).Value = Combciudad.Value
   Cells(llenar, 5).Value = Combedad.Value
   
 If Combciudad.Value = True Then
 
   Cells(llenar, 3).Value = "Femenino"

 Else
   
   Cells(llenar, 3).Value = "Masculino"
   
 End If
 
   
End Sub

Private Sub OptionButton1_Click()

End Sub

Private Sub Frame1_Click()

End Sub

Private Sub Label3_Click()

End Sub

Private Sub UserForm_Initialize()

 With Combciudad
 
  .AddItem "Barranquilla"
  .AddItem "Cartagena"
  .AddItem "Valledupar"
  .AddItem "Santa Marta"
  .AddItem "Bucaramanga"
 
 End With
  
  With Combedad
   
   .AddItem "18"
   .AddItem "17"
   .AddItem "16"
   .AddItem "15"
   
  End With

End Sub

	
	



