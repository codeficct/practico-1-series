<!-- # Practice-vb
This resposiory is to save projects practices of university UAGRM.
### Practice-1
[Practice-1-installator-app](https://github.com/satulio/practice-vb/blob/main/Practice-1/setup.exe)
 -->
 
 ```vb
 '<-- PRÁCTICO SERIES - UNIV. LUIS GABRIEL JANCO ALVAREZ -->'
Public Class Form1
    Dim errorMessage As String = "Dato incorrecto o faltante, se esperaba: "
    '<-- 1,2,3,4. GENERAR LA TABLA DE OPERACIONES DE N -->'
    Public Function SelectTable(n As Double, operatorString As String) As String
        Dim result, symbol As String
        Dim index As Integer
        Dim res As Double
        result = "" : symbol = ""
        For index = 0 To 10
            Select Case operatorString
                Case "*"
                    symbol = " *"
                    res = (index * n)
                Case "/"
                    symbol = " /"
                    res = (index / n)
                Case "+"
                    symbol = " +"
                    res = (index + n)
                Case "-"
                    symbol = " -"
                    res = (index - n)
            End Select
            result = result + Str(index) + symbol + Str(n) + " = " + Str(res) + Chr(13) + Chr(10)
        Next
        Return result
    End Function

    '<-- 5. SUMAR UNA SERIE REGULAR DE N TERMINOS -->'
    Public Function RegularSerie(n As UInt16, initialValue As Single, razon As Single, sumTotal As Boolean) As String
        Dim result As String = ""
        Dim index As UInt32
        Dim t, total As Single
        For index = 1 To n
            t = initialValue + (index - 1) * razon
            If sumTotal Then
                total += t
                result = Str(total)
            Else
                If index = n Then
                    result += Str(t)
                Else
                    result = result + Str(t) + "  + "
                End If
            End If
        Next
        Return "F = " + result
    End Function

    '<-- 6. SUMAR UNA SERIE DE N TERMINOS LOGARITMICA (Mejorar la suma) -->'
    Public Function LogarithmSerie(n As Integer, initialValue As Double, razon As Double, arg As Double, sumTotal As Boolean) As String
        Dim result As String = ""
        Dim count As Double
        Dim index As Integer
        Dim t, f, total As Double
        count = arg
        t = initialValue
        For index = 1 To n
            If sumTotal Then
                f = (Math.Log10(count) + index) / t
                total += f
                result = Str(total)
            Else
                If index.Equals(n) Then
                    result = result + "(ln(" + Str(count) + ") +" + Str(index) + ")/" + Str(t)
                Else
                    result = result + "(ln(" + Str(count) + ") +" + Str(index) + ")/" + Str(t) + " +  "
                End If
            End If
            count *= 10
            t = Math.Round(t + razon, 2)
        Next
        Return "F = " + result
    End Function

    '<-- 7. Icrement and Decrement or Progresive Serie and Regresive Serie -->'
    Public Function IncreaseAndDecrease(n As Integer, initialValueNumerator As Integer, initialValueDenominator As Integer, isSumTotal As Boolean) As String
        Dim result As String = ""
        Dim index As Integer
        Dim f, total As Double
        For index = 1 To n
            If isSumTotal Then
                f = (initialValueNumerator / initialValueDenominator)
                total += f
                result = Str(total)
            Else
                If index = n Then
                    result = result + Str(initialValueNumerator) + "/" + Str(initialValueDenominator)
                Else
                    result = result + Str(initialValueNumerator) + "/" + Str(initialValueDenominator) + " +  "
                End If
            End If
            initialValueNumerator -= index
            initialValueDenominator += index
        Next
        Return "F =" + result
    End Function

    '<-- 8. Regular serie with denominator factorial -->'
    Public Function Factorial(number As Double) As Double
        Dim fac As Double
        Dim index As Integer
        If number <> 0 Then
            fac = 1
            For index = Math.Abs(number) To 1 Step -1
                fac *= index
            Next
            If number < 0 Then
                fac = -fac
            End If
        Else
            fac = 1
        End If
        Return fac
    End Function
    Public Function RegularSerieWithFactorial(n As Integer, initialValueNum As Double, initialValueDen As Double, sumTotal As Double) As String
        Dim result As String = ""
        Dim index As Integer
        Dim t, f, total As Double
        For index = 0 To n
            If sumTotal Then
                If initialValueDen = 0 Then
                    f = 0
                Else
                    f = initialValueNum / (Factorial(initialValueDen) + initialValueDen)
                End If
                total += f
                result = Str(total)
            Else
                t = index + 1
                If index = n Then
                    result = result + Str(Math.Round(initialValueNum, 2)) + "/(!" + Str(initialValueDen) + "+" + Str(initialValueDen) + ")"
                Else
                    result = result + Str(Math.Round(initialValueNum, 2)) + "/(!" + Str(initialValueDen) + "+" + Str(initialValueDen) + ")  +  "
                End If
            End If
            initialValueNum -= (t / 100)
            initialValueDen += 1
        Next
        Return "F = " + result
    End Function
    '<-- 9. . F= X2/2! + X4/4! + X6/6!+… x, It is only an input variable that should be taken as a term -->'
    Public Function SumFactorial(n As Integer, x As Single, sumTotal As Boolean) As String
        Dim result As String = ""
        Dim index As Integer
        Dim formule As Double
        If n = 0 Then
            result = Str(0)
        End If
        For index = 1 To n
            If sumTotal Then
                formule = Math.Pow(x, index * 2) / Factorial(index * 2)
                result = Str(formule)
            Else
                If index = n Then
                    result = result + "(" + Str(x) + "^" + Str(index * 2) + ")/" + Str(index * 2) + "!"
                Else
                    result = result + "(" + Str(x) + "^" + Str(index * 2) + ")/" + Str(index * 2) + "! + "
                End If
            End If
        Next
        Return "F = " + result
    End Function

    '<-- 10. The argument of the root is a Fibonacci more a variablex1 -->
    Public Function SerieProgresiveFibonacci(n As Integer, x As Double, viRoot As Integer, sumTotal As Boolean) As String
        Dim result As String = ""
        Dim index, a, b, c, root As Integer
        Dim formule, total As Double
        a = -1 : b = 1 : root = viRoot
        For index = 1 To n
            c = a + b
            If sumTotal Then
                formule = (c + x) ^ (1 / root)
                total += formule
                result = Str(total)
            Else
                If index = n Then
                    result = result + Str(index * 3) + "√(" + Str(c) + "+" + Str(x) + ")"
                Else
                    result = result + Str(index * 3) + "√(" + Str(c) + "+" + Str(x) + ") + "
                End If
            End If
            a = b
            b = c
            root *= 3
        Next
        Return "F = " + result
    End Function

    '<-- 11. For tomorrow. :sleep i'm tired 
    Public Shared Function Pinponear(root As Double, vi As Double, razon As Double, sumTotal As Boolean) As String
        Dim result As String = ""
        Dim index As Integer
        Dim count, formule, total As Double
        count = vi
        For index = root To 2 Step -1
            If sumTotal Then
                formule = Math.Pow(Math.Cos(count), 1 / index)
                If index Mod 2 <> 0 Then
                    total = total - formule
                Else
                    total = total + formule
                End If
                result = Str(total)
            Else
                If index = 2 Then
                    result = result + Str(index) + "√cos(" + Str(count) + ")"
                Else
                    If index Mod 2 <> 0 Then
                        result = result + Str(index) + "√cos(" + Str(count) + ")  + "
                    Else
                        result = result + Str(index) + "√cos(" + Str(count) + ")  - "
                    End If
                End If
            End If
            count = Math.Round(count + razon, 2)
        Next
        Return "F = " + result
    End Function
    '<-- 12. - √(sin(0.1)/(3!/2)) + √(sin(0.11)/(3!/2))... También pimponea, resta y suma, resta y suma el termino -->'
    Public Function ProgresiveSeriePinponear(n As Integer, initValue As Double, r As Double, arg As Double, sumTotal As Boolean) As String
        Dim result As String = ""
        Dim index As Integer
        Dim total, formule, count As Double
        count = initValue
        For index = 1 To n
            If sumTotal Then
                formule = Math.Sqrt(Math.Sin(arg) / (Factorial(count) / 2))
                total = -total + formule
                result = Str(total)
            Else
                If index Mod 2 = 0 Then
                    result = result + "+ √sin(" + Str(arg) + ")/(" + Str(count) + "!/2) "
                Else
                    result = result + "- √sin(" + Str(arg) + ")/(" + Str(count) + "!/2) "
                End If
            End If
            arg = Math.Round(arg + r, 2)
            count += 3
        Next
        Return "F = " + result
    End Function

    '<-- 13. (π/2)/√(1000+0) + (π/1.9)/√(1001+1) + (π/1.8)/√(1003+1) El argumento de la raíz va en incremento en una progresión: Del 1ro al 2do 1; del 2do al 3ro 2; del 3ro al 4to 3; …mientras que el otro es Fibonacci.
    Public Function ProgresiveSerieFibonacci(n As Integer, initValue As Integer, sumTotal As Boolean) As String
        Dim result As String = ""
        Dim index As Integer
        Dim count, a, b, c, total, formule As Double
        count = 2 : a = -1 : b = 1
        For index = 1 To n
            c = a + b
            If sumTotal Then
                formule = (3.14159 / count) / Math.Sqrt(initValue + c)
                total += formule
                result = Str(total)
            Else
                If index = n Then
                    result = result + "(π/" + Str(count) + ")/√(" + Str(initValue) + "+" + Str(c) + ")"
                Else
                    result = result + "(π/" + Str(count) + ")/√(" + Str(initValue) + "+" + Str(c) + ")  +  "
                End If
            End If
            a = b
            b = c
            count = Math.Round(count - 0.1, 2)
            initValue += index
        Next
        Return "F = " + result
    End Function

    '<-- 14. 2√x^2/100 + 4√x^4/50 + 8√x^8/25... La raíz multiplica, mientras que el denominador dentro la raíz desdobla (divide) -->'
    Public Function SerieMultiplyAndUnfold(n As Integer, root As Double, num As Double, denom As Double, sumTotal As Boolean) As String
        Dim result As String = ""
        Dim index As Integer
        Dim total, formule As Double
        For index = 1 To n
            If sumTotal Then
                formule = Math.Pow(Math.Pow(num, root) / denom, 1 / root)
                total += formule
                result = Str(total)
            Else
                If index = n Then
                    result = result + Str(root) + "√(" + Str(num) + "^" + Str(root) + "/" + Str(denom) + ")"
                Else
                    result = result + Str(root) + "√(" + Str(num) + "^" + Str(root) + "/" + Str(denom) + ")  +  "
                End If
            End If
            root = Math.Round(root * 2, 2)
            denom = Math.Round(denom / 2, 2)
        Next
        Return "F = " + result
    End Function

    '<-- 15. (2+x^(1/16)) + (4+x^(1/14))... La base va doblando. OJO , HASTA QUE EL TERMINO DONDE X ELEVE A 1/2 -->'
    Public Function SerieBaseIsDoubling(n As Integer, base As Double, x As Double, denom As Double, sumTotal As Boolean) As String
        Dim result As String = ""
        Dim index As Integer
        Dim total, formule As Double
        For index = 1 To n
            If sumTotal Then
                formule = base + Math.Pow(x, 1 / denom)
                total += formule
                result = total
            Else
                If denom >= 2 Then
                    If index = n Then
                        result = result + "(" + Str(base) + "+" + Str(x) + "^(1/" + Str(denom) + "))"
                    Else
                        result = result + "(" + Str(base) + "+" + Str(x) + "^(1/" + Str(denom) + "))  + "
                    End If
                End If
            End If
            base *= 2
            denom -= 2
        Next
        Return "F = " + result
    End Function

    'examen
    Public Function AcumularTerminos(n As Integer, x As Integer, vi As Integer, sumTotal As Boolean) As String
        Dim result As String = ""
        Dim index, count As Integer
        Dim total, formule As Double
        count = 2
        For index = 0 To n
            If index <= 2 Then
                If sumTotal Then
                    formule = Math.Pow((Factorial(x + index) + (Math.PI / vi)) / Math.Pow(vi, n - index), 1 / (n - index))
                    total = -total + formule
                    result = Str(total)
                Else
                    If index Mod 2 = 0 Then
                        result = result + "(((x+" + Str(index) + ")!+π/" + Str(vi) + ")/" + Str(vi) + "^(n-" + Str(index) + "))^(1/(n-" + Str(index) + "))  -  "
                    Else
                        result = result + "(((x+" + Str(index) + ")!+π/" + Str(vi) + ")/" + Str(vi) + "^(n-" + Str(index) + "))^(1/(n-" + Str(index) + "))  +  "
                    End If
                End If
            End If
            vi = vi + count
            count = count * 2
        Next
        Return "F = " + result
    End Function

    '<-- Handle Clicks of menu buttons of designs. -->'
    Private Sub MultiplicarToolStripMenuItem_Click(sender As Object, e As EventArgs) Handles MultiplicarToolStripMenuItem.Click
        Try
            If IsNumeric(TextBox1.Text) Then
                Results.Text = SelectTable(CDbl(Val(TextBox1.Text)), "*")
            Else
                MsgBox(errorMessage + "número, en " + TextBox1.Name, Title:="1. Multiplicación.")
            End If
        Catch ex As Exception
            MsgBox(errorMessage + "números.")
        End Try
    End Sub

    Private Sub DivisionToolStripMenuItem_Click(sender As Object, e As EventArgs) Handles DivisionToolStripMenuItem.Click
        Try
            If IsNumeric(TextBox1.Text) Then
                Results.Text = SelectTable(CDbl(Val(TextBox1.Text)), "/")
            Else
                MsgBox(errorMessage + "número, en " + TextBox1.Name, Title:="2. División.")
            End If
        Catch ex As Exception
            MsgBox(errorMessage + "números.")
        End Try
    End Sub

    Private Sub SumaToolStripMenuItem_Click(sender As Object, e As EventArgs) Handles SumaToolStripMenuItem.Click
        Try
            If IsNumeric(TextBox1.Text) Then
                Results.Text = SelectTable(CDbl(Val(TextBox1.Text)), "+")
            Else
                MsgBox(errorMessage + "número, en " + TextBox1.Name, Title:="3. Suma.")
            End If
        Catch ex As Exception
            MsgBox(errorMessage + "números.")
        End Try
    End Sub

    Private Sub RestaToolStripMenuItem_Click(sender As Object, e As EventArgs) Handles RestaToolStripMenuItem.Click
        Try
            If IsNumeric(TextBox1.Text) Then
                Results.Text = SelectTable(CDbl(Val(TextBox1.Text)), "-")
            Else
                MsgBox(errorMessage + "número, en " + TextBox1.Name, Title:="4. Resta.")
            End If
        Catch ex As Exception
            MsgBox(errorMessage + "números.")
        End Try
    End Sub

    Private Sub SerieRegularToolStripMenuItem_Click(sender As Object, e As EventArgs) Handles SerieRegularToolStripMenuItem.Click
        Try
            Results.Text = RegularSerie(TextBox1.Text, TextBox2.Text, TextBox3.Text, True)
            Results2.Text = RegularSerie(TextBox1.Text, TextBox2.Text, TextBox3.Text, False)
        Catch ex As Exception
            MsgBox(errorMessage + "números.", Title:="5. Multiplicación.")
        End Try
    End Sub

    Private Sub Button1_Click(sender As Object, e As EventArgs) Handles Button1.Click
        TextBox1.Clear()
        TextBox2.Clear()
        TextBox3.Clear()
        TextBox4.Clear()
        Results2.Clear()
        Results.Clear()
    End Sub

    Private Sub SerieLogaritmoToolStripMenuItem_Click(sender As Object, e As EventArgs) Handles SerieLogaritmoToolStripMenuItem.Click
        Try
            If TextBox1.Text = "" Or TextBox2.Text = "" Or TextBox3.Text = "" Or TextBox4.Text = "" Then
                MsgBox(errorMessage + "número, en " + " los inputs.", Title:="6. Serie logaritmo.")
            Else
                Dim vi As Double = CDbl(Val(TextBox2.Text))
                Dim r As Double = CDbl(Val(TextBox3.Text))
                Dim arg As Double = CDbl(Val(TextBox4.Text))
                Results.Text = LogarithmSerie(TextBox1.Text, vi, r, arg, True)
                Results2.Text = LogarithmSerie(TextBox1.Text, vi, r, arg, False)
            End If
        Catch ex As Exception
            MsgBox(errorMessage + "números.", Title:="6. Serie logaritmo.")
        End Try
    End Sub

    Private Sub SerieProgresivaYRegresivaToolStripMenuItem_Click(sender As Object, e As EventArgs) Handles SerieProgresivaYRegresivaToolStripMenuItem.Click
        Try
            If TextBox1.Text = "" Or TextBox2.Text = "" Or TextBox3.Text = "" Then
                MsgBox(errorMessage + "número, en " + " los inputs.", Title:="7. Serie incremental.")
            Else
                Results.Text = IncreaseAndDecrease(TextBox1.Text, TextBox2.Text, TextBox3.Text, True)
                Results2.Text = IncreaseAndDecrease(TextBox1.Text, TextBox2.Text, TextBox3.Text, False)
            End If
        Catch ex As Exception
            MsgBox(errorMessage + "números.", Title:="7. Serie incremental.")
        End Try

    End Sub

    Private Sub SerieConFactorialToolStripMenuItem_Click(sender As Object, e As EventArgs) Handles SerieConFactorialToolStripMenuItem.Click
        Try
            If TextBox1.Text = "" Or TextBox2.Text = "" Or TextBox3.Text = "" Then
                MsgBox(errorMessage + "números en los inputs.", Title:="8. Serie eegresiva con factorial.")
            Else
                Dim vi As Double = CDbl(Val(TextBox2.Text))
                Dim r As Double = CDbl(Val(TextBox3.Text))
                Results.Text = RegularSerieWithFactorial(TextBox1.Text, vi, r, True)
                Results2.Text = RegularSerieWithFactorial(TextBox1.Text, vi, r, False)
            End If
        Catch ex As Exception
            MsgBox(errorMessage + "números.", Title:="8. Serie regresiva con factorial.")
        End Try
    End Sub

    Private Sub SerieToolStripMenuItem_Click(sender As Object, e As EventArgs) Handles SerieToolStripMenuItem.Click
        Try
            Results.Text = SumFactorial(TextBox1.Text, TextBox2.Text, True)
            Results2.Text = SumFactorial(TextBox1.Text, TextBox2.Text, False)
        Catch ex As Exception
            MsgBox(errorMessage + "números.", Title:="9. Serie X, con factorial.")
        End Try
    End Sub

    Private Sub SerieProgresivaConFibonacciToolStripMenuItem_Click(sender As Object, e As EventArgs) Handles SerieProgresivaConFibonacciToolStripMenuItem.Click
        Try
            Results.Text = SerieProgresiveFibonacci(TextBox1.Text, TextBox2.Text, TextBox3.Text, True)
            Results2.Text = SerieProgresiveFibonacci(TextBox1.Text, TextBox2.Text, TextBox3.Text, False)
        Catch ex As Exception
            MsgBox(errorMessage + "números.", Title:="10. Serie acumulativa con fibonacci.")
        End Try
    End Sub

    Private Sub SerieRegularPinponearToolStripMenuItem_Click(sender As Object, e As EventArgs) Handles SerieRegularPinponearToolStripMenuItem.Click
        Try
            Dim vi As Double = CDbl(Val(TextBox2.Text))
            Dim r As Double = CDbl(Val(TextBox3.Text))
            Results.Text = Pinponear(TextBox1.Text, vi, r, True)
            Results2.Text = Pinponear(TextBox1.Text, vi, r, False)
        Catch ex As Exception
            MsgBox(errorMessage + "números.", Title:="11. Serie regular pinponea.")
        End Try
    End Sub

    Private Sub SerieAcumulativaPinponeaToolStripMenuItem_Click(sender As Object, e As EventArgs) Handles SerieAcumulativaPinponeaToolStripMenuItem.Click
        Try
            Dim vi As Double = CDbl(Val(TextBox2.Text))
            Dim r As Double = CDbl(Val(TextBox3.Text))
            Dim arg As Double = CDbl(Val(TextBox4.Text))
            Results.Text = ProgresiveSeriePinponear(TextBox1.Text, vi, r, arg, True)
            Results2.Text = ProgresiveSeriePinponear(TextBox1.Text, vi, r, arg, False)
        Catch ex As Exception
            MsgBox(errorMessage + "números.", Title:="12. Serie acumulativa pinponea.")
        End Try
    End Sub

    Private Sub ToolStripMenuItem2_Click(sender As Object, e As EventArgs) Handles ToolStripMenuItem2.Click
        Try
            Results.Text = ProgresiveSerieFibonacci(TextBox1.Text, TextBox2.Text, True)
            Results2.Text = ProgresiveSerieFibonacci(TextBox1.Text, TextBox2.Text, False)
        Catch ex As Exception
            MsgBox(errorMessage + "números.", Title:="13. Serie de incremento con fibonacci.")
        End Try
    End Sub

    Private Sub SerieToolStripMenuItem1_Click(sender As Object, e As EventArgs) Handles SerieToolStripMenuItem1.Click
        Try
            Dim vi As Double = CDbl(Val(TextBox2.Text))
            Dim r As Double = CDbl(Val(TextBox3.Text))
            Dim arg As Double = CDbl(Val(TextBox4.Text))
            Results.Text = SerieMultiplyAndUnfold(TextBox1.Text, vi, r, arg, True)
            Results2.Text = SerieMultiplyAndUnfold(TextBox1.Text, vi, r, arg, False)
        Catch ex As Exception
            MsgBox(errorMessage + "números.", Title:="14. Serie raiz, multiplica y reduce (desdobla).")
        End Try
    End Sub

    Private Sub SerieBaseVaDoblandoToolStripMenuItem_Click(sender As Object, e As EventArgs) Handles SerieBaseVaDoblandoToolStripMenuItem.Click
        Try
            Dim vi As Double = CDbl(Val(TextBox2.Text))
            Dim r As Double = CDbl(Val(TextBox3.Text))
            Dim arg As Double = CDbl(Val(TextBox4.Text))
            Results.Text = SerieBaseIsDoubling(TextBox1.Text, vi, r, arg, True)
            Results2.Text = SerieBaseIsDoubling(TextBox1.Text, vi, r, arg, False)
        Catch ex As Exception
            MsgBox(errorMessage + "números.", Title:="15. Serie progresiva, base va doblando.")
        End Try
    End Sub

    Private Sub AcumularTerminoToolStripMenuItem_Click(sender As Object, e As EventArgs) Handles AcumularTerminoToolStripMenuItem.Click
        Try
            Results.Text = AcumularTerminos(TextBox1.Text, TextBox2.Text, TextBox3.Text, True)
            Results2.Text = AcumularTerminos(TextBox1.Text, TextBox2.Text, TextBox3.Text, False)
        Catch ex As Exception
            MsgBox(errorMessage + "números.")
        End Try
    End Sub
End Class

 ```
