<!-- # Practice-vb
This resposiory is to save projects practices of university UAGRM.
### Practice-1
[Practice-1-installator-app](https://github.com/satulio/practice-vb/blob/main/Practice-1/setup.exe)
 -->
 
 ```vb
 <Global.Microsoft.VisualBasic.CompilerServices.DesignerGenerated()>
Partial Class Form1
    Inherits System.Windows.Forms.Form

    'Form overrides dispose to clean up the component list.
    <System.Diagnostics.DebuggerNonUserCode()>
    Protected Overrides Sub Dispose(ByVal disposing As Boolean)
        Try
            If disposing AndAlso components IsNot Nothing Then
                components.Dispose()
            End If
        Finally
            MyBase.Dispose(disposing)
        End Try
    End Sub

    'Required by the Windows Form Designer
    Private components As System.ComponentModel.IContainer

    'NOTE: The following procedure is required by the Windows Form Designer
    'It can be modified using the Windows Form Designer.  
    'Do not modify it using the code editor.
    <System.Diagnostics.DebuggerStepThrough()>
    Private Sub InitializeComponent()
        Me.Label1 = New System.Windows.Forms.Label()
        Me.MenuStrip1 = New System.Windows.Forms.MenuStrip()
        Me.OperacionesToolStripMenuItem = New System.Windows.Forms.ToolStripMenuItem()
        Me.MultiplicarToolStripMenuItem = New System.Windows.Forms.ToolStripMenuItem()
        Me.DivisionToolStripMenuItem = New System.Windows.Forms.ToolStripMenuItem()
        Me.SumaToolStripMenuItem = New System.Windows.Forms.ToolStripMenuItem()
        Me.RestaToolStripMenuItem = New System.Windows.Forms.ToolStripMenuItem()
        Me.SeriesToolStripMenuItem = New System.Windows.Forms.ToolStripMenuItem()
        Me.SerieRegularToolStripMenuItem = New System.Windows.Forms.ToolStripMenuItem()
        Me.SerieLogaritmoToolStripMenuItem = New System.Windows.Forms.ToolStripMenuItem()
        Me.SerieProgresivaYRegresivaToolStripMenuItem = New System.Windows.Forms.ToolStripMenuItem()
        Me.SerieConFactorialToolStripMenuItem = New System.Windows.Forms.ToolStripMenuItem()
        Me.SerieToolStripMenuItem = New System.Windows.Forms.ToolStripMenuItem()
        Me.SerieProgresivaConFibonacciToolStripMenuItem = New System.Windows.Forms.ToolStripMenuItem()
        Me.SerieRegularPinponearToolStripMenuItem = New System.Windows.Forms.ToolStripMenuItem()
        Me.SerieAcumulativaPinponeaToolStripMenuItem = New System.Windows.Forms.ToolStripMenuItem()
        Me.ToolStripMenuItem2 = New System.Windows.Forms.ToolStripMenuItem()
        Me.SerieToolStripMenuItem1 = New System.Windows.Forms.ToolStripMenuItem()
        Me.SerieBaseVaDoblandoToolStripMenuItem = New System.Windows.Forms.ToolStripMenuItem()
        Me.ParcialToolStripMenuItem = New System.Windows.Forms.ToolStripMenuItem()
        Me.AcumularTerminoToolStripMenuItem = New System.Windows.Forms.ToolStripMenuItem()
        Me.TextBox1 = New System.Windows.Forms.TextBox()
        Me.TextBox2 = New System.Windows.Forms.TextBox()
        Me.TextBox3 = New System.Windows.Forms.TextBox()
        Me.Results = New System.Windows.Forms.TextBox()
        Me.Button1 = New System.Windows.Forms.Button()
        Me.Results2 = New System.Windows.Forms.TextBox()
        Me.Label3 = New System.Windows.Forms.Label()
        Me.Label2 = New System.Windows.Forms.Label()
        Me.Label4 = New System.Windows.Forms.Label()
        Me.Label5 = New System.Windows.Forms.Label()
        Me.Label6 = New System.Windows.Forms.Label()
        Me.Label7 = New System.Windows.Forms.Label()
        Me.Label8 = New System.Windows.Forms.Label()
        Me.Label9 = New System.Windows.Forms.Label()
        Me.Label10 = New System.Windows.Forms.Label()
        Me.Label11 = New System.Windows.Forms.Label()
        Me.Label12 = New System.Windows.Forms.Label()
        Me.Label13 = New System.Windows.Forms.Label()
        Me.TextBox4 = New System.Windows.Forms.TextBox()
        Me.Label14 = New System.Windows.Forms.Label()
        Me.Label16 = New System.Windows.Forms.Label()
        Me.Label15 = New System.Windows.Forms.Label()
        Me.Label17 = New System.Windows.Forms.Label()
        Me.MenuStrip1.SuspendLayout()
        Me.SuspendLayout()
        '
        'Label1
        '
        Me.Label1.AutoSize = True
        Me.Label1.BackColor = System.Drawing.Color.Transparent
        Me.Label1.Font = New System.Drawing.Font("Segoe UI", 12.0!, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point)
        Me.Label1.ForeColor = System.Drawing.Color.FromArgb(CType(CType(34, Byte), Integer), CType(CType(34, Byte), Integer), CType(CType(34, Byte), Integer))
        Me.Label1.Location = New System.Drawing.Point(602, 2)
        Me.Label1.Margin = New System.Windows.Forms.Padding(4, 0, 4, 0)
        Me.Label1.Name = "Label1"
        Me.Label1.Size = New System.Drawing.Size(242, 21)
        Me.Label1.TabIndex = 0
        Me.Label1.Text = "Prático Series - Ing. Alberto Mollo"
        '
        'MenuStrip1
        '
        Me.MenuStrip1.Items.AddRange(New System.Windows.Forms.ToolStripItem() {Me.OperacionesToolStripMenuItem, Me.SeriesToolStripMenuItem, Me.ParcialToolStripMenuItem})
        Me.MenuStrip1.Location = New System.Drawing.Point(0, 0)
        Me.MenuStrip1.Name = "MenuStrip1"
        Me.MenuStrip1.Size = New System.Drawing.Size(857, 24)
        Me.MenuStrip1.TabIndex = 1
        Me.MenuStrip1.Text = "MenuStrip1"
        '
        'OperacionesToolStripMenuItem
        '
        Me.OperacionesToolStripMenuItem.DropDownItems.AddRange(New System.Windows.Forms.ToolStripItem() {Me.MultiplicarToolStripMenuItem, Me.DivisionToolStripMenuItem, Me.SumaToolStripMenuItem, Me.RestaToolStripMenuItem})
        Me.OperacionesToolStripMenuItem.Name = "OperacionesToolStripMenuItem"
        Me.OperacionesToolStripMenuItem.Size = New System.Drawing.Size(85, 20)
        Me.OperacionesToolStripMenuItem.Text = "Operaciones"
        '
        'MultiplicarToolStripMenuItem
        '
        Me.MultiplicarToolStripMenuItem.Name = "MultiplicarToolStripMenuItem"
        Me.MultiplicarToolStripMenuItem.Size = New System.Drawing.Size(143, 22)
        Me.MultiplicarToolStripMenuItem.Text = "1. Multiplicar"
        '
        'DivisionToolStripMenuItem
        '
        Me.DivisionToolStripMenuItem.Name = "DivisionToolStripMenuItem"
        Me.DivisionToolStripMenuItem.Size = New System.Drawing.Size(143, 22)
        Me.DivisionToolStripMenuItem.Text = "2. Division"
        '
        'SumaToolStripMenuItem
        '
        Me.SumaToolStripMenuItem.Name = "SumaToolStripMenuItem"
        Me.SumaToolStripMenuItem.Size = New System.Drawing.Size(143, 22)
        Me.SumaToolStripMenuItem.Text = "3. Suma"
        '
        'RestaToolStripMenuItem
        '
        Me.RestaToolStripMenuItem.Name = "RestaToolStripMenuItem"
        Me.RestaToolStripMenuItem.Size = New System.Drawing.Size(143, 22)
        Me.RestaToolStripMenuItem.Text = "4. Resta"
        '
        'SeriesToolStripMenuItem
        '
        Me.SeriesToolStripMenuItem.DropDownItems.AddRange(New System.Windows.Forms.ToolStripItem() {Me.SerieRegularToolStripMenuItem, Me.SerieLogaritmoToolStripMenuItem, Me.SerieProgresivaYRegresivaToolStripMenuItem, Me.SerieConFactorialToolStripMenuItem, Me.SerieToolStripMenuItem, Me.SerieProgresivaConFibonacciToolStripMenuItem, Me.SerieRegularPinponearToolStripMenuItem, Me.SerieAcumulativaPinponeaToolStripMenuItem, Me.ToolStripMenuItem2, Me.SerieToolStripMenuItem1, Me.SerieBaseVaDoblandoToolStripMenuItem})
        Me.SeriesToolStripMenuItem.Name = "SeriesToolStripMenuItem"
        Me.SeriesToolStripMenuItem.Size = New System.Drawing.Size(49, 20)
        Me.SeriesToolStripMenuItem.Text = "Series"
        '
        'SerieRegularToolStripMenuItem
        '
        Me.SerieRegularToolStripMenuItem.Name = "SerieRegularToolStripMenuItem"
        Me.SerieRegularToolStripMenuItem.Size = New System.Drawing.Size(272, 22)
        Me.SerieRegularToolStripMenuItem.Text = "5. Serie Regular"
        '
        'SerieLogaritmoToolStripMenuItem
        '
        Me.SerieLogaritmoToolStripMenuItem.Name = "SerieLogaritmoToolStripMenuItem"
        Me.SerieLogaritmoToolStripMenuItem.Size = New System.Drawing.Size(272, 22)
        Me.SerieLogaritmoToolStripMenuItem.Text = "6. Serie Logaritmo"
        '
        'SerieProgresivaYRegresivaToolStripMenuItem
        '
        Me.SerieProgresivaYRegresivaToolStripMenuItem.Name = "SerieProgresivaYRegresivaToolStripMenuItem"
        Me.SerieProgresivaYRegresivaToolStripMenuItem.Size = New System.Drawing.Size(272, 22)
        Me.SerieProgresivaYRegresivaToolStripMenuItem.Text = "7. Serie Incremental"
        '
        'SerieConFactorialToolStripMenuItem
        '
        Me.SerieConFactorialToolStripMenuItem.Name = "SerieConFactorialToolStripMenuItem"
        Me.SerieConFactorialToolStripMenuItem.Size = New System.Drawing.Size(272, 22)
        Me.SerieConFactorialToolStripMenuItem.Text = "8. Serie regresiva con factorial"
        '
        'SerieToolStripMenuItem
        '
        Me.SerieToolStripMenuItem.Name = "SerieToolStripMenuItem"
        Me.SerieToolStripMenuItem.Size = New System.Drawing.Size(272, 22)
        Me.SerieToolStripMenuItem.Text = "9. Serie X, factorial"
        '
        'SerieProgresivaConFibonacciToolStripMenuItem
        '
        Me.SerieProgresivaConFibonacciToolStripMenuItem.Name = "SerieProgresivaConFibonacciToolStripMenuItem"
        Me.SerieProgresivaConFibonacciToolStripMenuItem.Size = New System.Drawing.Size(272, 22)
        Me.SerieProgresivaConFibonacciToolStripMenuItem.Text = "10. Serie acumulativa con fibonacci"
        '
        'SerieRegularPinponearToolStripMenuItem
        '
        Me.SerieRegularPinponearToolStripMenuItem.Name = "SerieRegularPinponearToolStripMenuItem"
        Me.SerieRegularPinponearToolStripMenuItem.Size = New System.Drawing.Size(272, 22)
        Me.SerieRegularPinponearToolStripMenuItem.Text = "11. Serie regular - pinponea"
        '
        'SerieAcumulativaPinponeaToolStripMenuItem
        '
        Me.SerieAcumulativaPinponeaToolStripMenuItem.Name = "SerieAcumulativaPinponeaToolStripMenuItem"
        Me.SerieAcumulativaPinponeaToolStripMenuItem.Size = New System.Drawing.Size(272, 22)
        Me.SerieAcumulativaPinponeaToolStripMenuItem.Text = "12. Serie acumulativa - pinponea"
        '
        'ToolStripMenuItem2
        '
        Me.ToolStripMenuItem2.Name = "ToolStripMenuItem2"
        Me.ToolStripMenuItem2.Size = New System.Drawing.Size(272, 22)
        Me.ToolStripMenuItem2.Text = "13. Serie de incremento con fibonacci"
        '
        'SerieToolStripMenuItem1
        '
        Me.SerieToolStripMenuItem1.Name = "SerieToolStripMenuItem1"
        Me.SerieToolStripMenuItem1.Size = New System.Drawing.Size(272, 22)
        Me.SerieToolStripMenuItem1.Text = "14. Serie raiz multiplica y desdobla"
        '
        'SerieBaseVaDoblandoToolStripMenuItem
        '
        Me.SerieBaseVaDoblandoToolStripMenuItem.Name = "SerieBaseVaDoblandoToolStripMenuItem"
        Me.SerieBaseVaDoblandoToolStripMenuItem.Size = New System.Drawing.Size(272, 22)
        Me.SerieBaseVaDoblandoToolStripMenuItem.Text = "15. Serie Pr. base va doblando"
        '
        'ParcialToolStripMenuItem
        '
        Me.ParcialToolStripMenuItem.DropDownItems.AddRange(New System.Windows.Forms.ToolStripItem() {Me.AcumularTerminoToolStripMenuItem})
        Me.ParcialToolStripMenuItem.Name = "ParcialToolStripMenuItem"
        Me.ParcialToolStripMenuItem.Size = New System.Drawing.Size(54, 20)
        Me.ParcialToolStripMenuItem.Text = "Parcial"
        '
        'AcumularTerminoToolStripMenuItem
        '
        Me.AcumularTerminoToolStripMenuItem.Name = "AcumularTerminoToolStripMenuItem"
        Me.AcumularTerminoToolStripMenuItem.Size = New System.Drawing.Size(184, 22)
        Me.AcumularTerminoToolStripMenuItem.Text = "1. Acumular Termino"
        '
        'TextBox1
        '
        Me.TextBox1.BackColor = System.Drawing.Color.FromArgb(CType(CType(192, Byte), Integer), CType(CType(255, Byte), Integer), CType(CType(255, Byte), Integer))
        Me.TextBox1.Location = New System.Drawing.Point(306, 42)
        Me.TextBox1.Name = "TextBox1"
        Me.TextBox1.Size = New System.Drawing.Size(100, 29)
        Me.TextBox1.TabIndex = 2
        '
        'TextBox2
        '
        Me.TextBox2.BackColor = System.Drawing.Color.FromArgb(CType(CType(192, Byte), Integer), CType(CType(255, Byte), Integer), CType(CType(255, Byte), Integer))
        Me.TextBox2.Location = New System.Drawing.Point(412, 42)
        Me.TextBox2.Name = "TextBox2"
        Me.TextBox2.Size = New System.Drawing.Size(100, 29)
        Me.TextBox2.TabIndex = 3
        '
        'TextBox3
        '
        Me.TextBox3.BackColor = System.Drawing.Color.FromArgb(CType(CType(192, Byte), Integer), CType(CType(255, Byte), Integer), CType(CType(255, Byte), Integer))
        Me.TextBox3.Location = New System.Drawing.Point(518, 42)
        Me.TextBox3.Name = "TextBox3"
        Me.TextBox3.Size = New System.Drawing.Size(100, 29)
        Me.TextBox3.TabIndex = 4
        '
        'Results
        '
        Me.Results.BackColor = System.Drawing.Color.FromArgb(CType(CType(238, Byte), Integer), CType(CType(238, Byte), Integer), CType(CType(238, Byte), Integer))
        Me.Results.BorderStyle = System.Windows.Forms.BorderStyle.FixedSingle
        Me.Results.Location = New System.Drawing.Point(306, 77)
        Me.Results.Multiline = True
        Me.Results.Name = "Results"
        Me.Results.ReadOnly = True
        Me.Results.ScrollBars = System.Windows.Forms.ScrollBars.Vertical
        Me.Results.Size = New System.Drawing.Size(529, 211)
        Me.Results.TabIndex = 5
        '
        'Button1
        '
        Me.Button1.BackColor = System.Drawing.Color.FromArgb(CType(CType(0, Byte), Integer), CType(CType(153, Byte), Integer), CType(CType(255, Byte), Integer))
        Me.Button1.FlatAppearance.BorderColor = System.Drawing.Color.FromArgb(CType(CType(0, Byte), Integer), CType(CType(153, Byte), Integer), CType(CType(255, Byte), Integer))
        Me.Button1.Font = New System.Drawing.Font("Segoe UI", 10.0!, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point)
        Me.Button1.ForeColor = System.Drawing.Color.White
        Me.Button1.Location = New System.Drawing.Point(760, 434)
        Me.Button1.Name = "Button1"
        Me.Button1.Size = New System.Drawing.Size(75, 28)
        Me.Button1.TabIndex = 8
        Me.Button1.Text = "Reset"
        Me.Button1.UseVisualStyleBackColor = False
        '
        'Results2
        '
        Me.Results2.BorderStyle = System.Windows.Forms.BorderStyle.FixedSingle
        Me.Results2.Font = New System.Drawing.Font("Segoe UI", 12.0!, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point)
        Me.Results2.Location = New System.Drawing.Point(306, 304)
        Me.Results2.Multiline = True
        Me.Results2.Name = "Results2"
        Me.Results2.ReadOnly = True
        Me.Results2.ScrollBars = System.Windows.Forms.ScrollBars.Horizontal
        Me.Results2.Size = New System.Drawing.Size(529, 97)
        Me.Results2.TabIndex = 10
        Me.Results2.WordWrap = False
        '
        'Label3
        '
        Me.Label3.AutoSize = True
        Me.Label3.Font = New System.Drawing.Font("Segoe UI", 10.0!, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point)
        Me.Label3.ForeColor = System.Drawing.Color.DimGray
        Me.Label3.Location = New System.Drawing.Point(12, 59)
        Me.Label3.Name = "Label3"
        Me.Label3.Size = New System.Drawing.Size(233, 38)
        Me.Label3.TabIndex = 7
        Me.Label3.Text = "5. Serie regular sumar n terminos." & Global.Microsoft.VisualBasic.ChrW(13) & Global.Microsoft.VisualBasic.ChrW(10) & "     n terminos, vi valor inicial, r razon"
        '
        'Label2
        '
        Me.Label2.AutoSize = True
        Me.Label2.Font = New System.Drawing.Font("Segoe UI", 10.0!, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point)
        Me.Label2.ForeColor = System.Drawing.Color.Black
        Me.Label2.Location = New System.Drawing.Point(12, 38)
        Me.Label2.Name = "Label2"
        Me.Label2.Size = New System.Drawing.Size(231, 19)
        Me.Label2.TabIndex = 6
        Me.Label2.Text = "1, 2, 3, 4. Genera operaciones de ""n"""
        '
        'Label4
        '
        Me.Label4.AutoSize = True
        Me.Label4.Font = New System.Drawing.Font("Segoe UI", 10.0!, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point)
        Me.Label4.ForeColor = System.Drawing.Color.DimGray
        Me.Label4.Location = New System.Drawing.Point(12, 155)
        Me.Label4.Name = "Label4"
        Me.Label4.Size = New System.Drawing.Size(260, 76)
        Me.Label4.TabIndex = 9
        Me.Label4.Text = "7. Genera la serie que decrementa" & Global.Microsoft.VisualBasic.ChrW(13) & Global.Microsoft.VisualBasic.ChrW(10) & "    y incrementa sus valores." & Global.Microsoft.VisualBasic.ChrW(13) & Global.Microsoft.VisualBasic.ChrW(10) & "   (n terminos," &
    " vi: Valor inicial Numerador," & Global.Microsoft.VisualBasic.ChrW(13) & Global.Microsoft.VisualBasic.ChrW(10) & "    r: Valor inicial Denominador)."
        '
        'Label5
        '
        Me.Label5.AutoSize = True
        Me.Label5.Font = New System.Drawing.Font("Segoe UI", 10.0!, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point)
        Me.Label5.ForeColor = System.Drawing.Color.Black
        Me.Label5.Location = New System.Drawing.Point(12, 98)
        Me.Label5.Name = "Label5"
        Me.Label5.Size = New System.Drawing.Size(274, 57)
        Me.Label5.TabIndex = 11
        Me.Label5.Text = "6. Genera la suma de una serie acumulativa" & Global.Microsoft.VisualBasic.ChrW(13) & Global.Microsoft.VisualBasic.ChrW(10) & "    de (n: term., vi: valor init. den" &
    "ominador," & Global.Microsoft.VisualBasic.ChrW(13) & Global.Microsoft.VisualBasic.ChrW(10) & "    r: razon de incremento, arg: args del log)"
        '
        'Label6
        '
        Me.Label6.AutoSize = True
        Me.Label6.Font = New System.Drawing.Font("Segoe UI", 10.0!, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point)
        Me.Label6.ForeColor = System.Drawing.Color.Black
        Me.Label6.Location = New System.Drawing.Point(12, 231)
        Me.Label6.Name = "Label6"
        Me.Label6.Size = New System.Drawing.Size(279, 57)
        Me.Label6.TabIndex = 12
        Me.Label6.Text = "8. Serie regresiva, con denominador factorial" & Global.Microsoft.VisualBasic.ChrW(13) & Global.Microsoft.VisualBasic.ChrW(10) & "    (n terminos, vi: valor inicial" &
    " numerador, " & Global.Microsoft.VisualBasic.ChrW(13) & Global.Microsoft.VisualBasic.ChrW(10) & "     r: valor inicial denominador)."
        '
        'Label7
        '
        Me.Label7.AutoSize = True
        Me.Label7.Font = New System.Drawing.Font("Segoe UI", 8.0!, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point)
        Me.Label7.ForeColor = System.Drawing.Color.DarkGray
        Me.Label7.Location = New System.Drawing.Point(306, 26)
        Me.Label7.Name = "Label7"
        Me.Label7.Size = New System.Drawing.Size(14, 13)
        Me.Label7.TabIndex = 13
        Me.Label7.Text = "n"
        '
        'Label8
        '
        Me.Label8.AutoSize = True
        Me.Label8.Font = New System.Drawing.Font("Segoe UI", 8.0!, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point)
        Me.Label8.ForeColor = System.Drawing.Color.DarkGray
        Me.Label8.Location = New System.Drawing.Point(412, 26)
        Me.Label8.Name = "Label8"
        Me.Label8.Size = New System.Drawing.Size(15, 13)
        Me.Label8.TabIndex = 14
        Me.Label8.Text = "vi"
        '
        'Label9
        '
        Me.Label9.AutoSize = True
        Me.Label9.Font = New System.Drawing.Font("Segoe UI", 8.0!, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point)
        Me.Label9.ForeColor = System.Drawing.Color.DarkGray
        Me.Label9.Location = New System.Drawing.Point(518, 26)
        Me.Label9.Name = "Label9"
        Me.Label9.Size = New System.Drawing.Size(11, 13)
        Me.Label9.TabIndex = 15
        Me.Label9.Text = "r"
        '
        'Label10
        '
        Me.Label10.AutoSize = True
        Me.Label10.Font = New System.Drawing.Font("Segoe UI", 10.0!, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point)
        Me.Label10.ForeColor = System.Drawing.Color.DimGray
        Me.Label10.Location = New System.Drawing.Point(12, 288)
        Me.Label10.Name = "Label10"
        Me.Label10.Size = New System.Drawing.Size(199, 38)
        Me.Label10.TabIndex = 16
        Me.Label10.Text = "9. Serie progresiva con factorial" & Global.Microsoft.VisualBasic.ChrW(13) & Global.Microsoft.VisualBasic.ChrW(10) & "    (n: terminos, vi: valor de x)"
        '
        'Label11
        '
        Me.Label11.AutoSize = True
        Me.Label11.Font = New System.Drawing.Font("Segoe UI", 10.0!, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point)
        Me.Label11.ForeColor = System.Drawing.Color.Black
        Me.Label11.Location = New System.Drawing.Point(12, 326)
        Me.Label11.Name = "Label11"
        Me.Label11.Size = New System.Drawing.Size(239, 57)
        Me.Label11.TabIndex = 17
        Me.Label11.Text = "10. Serie acumulativa con Fibonacci," & Global.Microsoft.VisualBasic.ChrW(13) & Global.Microsoft.VisualBasic.ChrW(10) & "      (n: terminos, vi: valor para x, " & Global.Microsoft.VisualBasic.ChrW(13) & Global.Microsoft.VisualBasic.ChrW(10) & "   " &
    "    r: valor inicial del indice de la raiz)"
        '
        'Label12
        '
        Me.Label12.AutoSize = True
        Me.Label12.Font = New System.Drawing.Font("Segoe UI", 10.0!, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point)
        Me.Label12.ForeColor = System.Drawing.Color.DimGray
        Me.Label12.Location = New System.Drawing.Point(12, 383)
        Me.Label12.Name = "Label12"
        Me.Label12.Size = New System.Drawing.Size(225, 57)
        Me.Label12.TabIndex = 18
        Me.Label12.Text = "11. Pinponea la serie..." & Global.Microsoft.VisualBasic.ChrW(13) & Global.Microsoft.VisualBasic.ChrW(10) & "   (n: raiz inicial, vi: arg del seno" & Global.Microsoft.VisualBasic.ChrW(13) & Global.Microsoft.VisualBasic.ChrW(10) & "    r: razon de " &
    "incremento del seno)."
        '
        'Label13
        '
        Me.Label13.AutoSize = True
        Me.Label13.Font = New System.Drawing.Font("Segoe UI", 8.0!, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point)
        Me.Label13.ForeColor = System.Drawing.Color.DarkGray
        Me.Label13.Location = New System.Drawing.Point(624, 26)
        Me.Label13.Name = "Label13"
        Me.Label13.Size = New System.Drawing.Size(24, 13)
        Me.Label13.TabIndex = 20
        Me.Label13.Text = "arg"
        '
        'TextBox4
        '
        Me.TextBox4.BackColor = System.Drawing.Color.FromArgb(CType(CType(192, Byte), Integer), CType(CType(255, Byte), Integer), CType(CType(255, Byte), Integer))
        Me.TextBox4.Location = New System.Drawing.Point(624, 42)
        Me.TextBox4.Name = "TextBox4"
        Me.TextBox4.Size = New System.Drawing.Size(100, 29)
        Me.TextBox4.TabIndex = 19
        '
        'Label14
        '
        Me.Label14.AutoSize = True
        Me.Label14.Font = New System.Drawing.Font("Segoe UI", 10.0!, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point)
        Me.Label14.ForeColor = System.Drawing.Color.Black
        Me.Label14.Location = New System.Drawing.Point(12, 440)
        Me.Label14.Name = "Label14"
        Me.Label14.Size = New System.Drawing.Size(256, 76)
        Me.Label14.TabIndex = 21
        Me.Label14.Text = "12. Serie progresiva pinponea (-, +, -, +)" & Global.Microsoft.VisualBasic.ChrW(13) & Global.Microsoft.VisualBasic.ChrW(10) & "      (n: terminos, vi: valor inicial" &
    " factorial, " & Global.Microsoft.VisualBasic.ChrW(13) & Global.Microsoft.VisualBasic.ChrW(10) & "       r: razon de incremento del sin()," & Global.Microsoft.VisualBasic.ChrW(13) & Global.Microsoft.VisualBasic.ChrW(10) & "       arg: valor inicia" &
    "l del arg del sin(...))."
        '
        'Label16
        '
        Me.Label16.AutoSize = True
        Me.Label16.Font = New System.Drawing.Font("Segoe UI", 10.0!, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point)
        Me.Label16.ForeColor = System.Drawing.Color.DimGray
        Me.Label16.Location = New System.Drawing.Point(12, 516)
        Me.Label16.Name = "Label16"
        Me.Label16.Size = New System.Drawing.Size(308, 38)
        Me.Label16.TabIndex = 23
        Me.Label16.Text = "13. Incremento de una progresion con fibonacci" & Global.Microsoft.VisualBasic.ChrW(13) & Global.Microsoft.VisualBasic.ChrW(10) & "      (n: terminos, vi: valor ini" &
    "cial del arg de la raiz)."
        '
        'Label15
        '
        Me.Label15.AutoSize = True
        Me.Label15.Font = New System.Drawing.Font("Segoe UI", 10.0!, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point)
        Me.Label15.ForeColor = System.Drawing.Color.Black
        Me.Label15.Location = New System.Drawing.Point(12, 554)
        Me.Label15.Name = "Label15"
        Me.Label15.Size = New System.Drawing.Size(292, 57)
        Me.Label15.TabIndex = 24
        Me.Label15.Text = "14. La raíz multiplica y denominador desdobla," & Global.Microsoft.VisualBasic.ChrW(13) & Global.Microsoft.VisualBasic.ChrW(10) & "      (n: terminos, vi: raiz inic" &
    "ial, r: numerador," & Global.Microsoft.VisualBasic.ChrW(13) & Global.Microsoft.VisualBasic.ChrW(10) & "       arg: denominador)."
        '
        'Label17
        '
        Me.Label17.AutoSize = True
        Me.Label17.Font = New System.Drawing.Font("Segoe UI", 10.0!, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point)
        Me.Label17.ForeColor = System.Drawing.Color.DimGray
        Me.Label17.Location = New System.Drawing.Point(12, 611)
        Me.Label17.Name = "Label17"
        Me.Label17.Size = New System.Drawing.Size(393, 38)
        Me.Label17.TabIndex = 25
        Me.Label17.Text = "15. Serie progresiva cuando la base va doblando," & Global.Microsoft.VisualBasic.ChrW(13) & Global.Microsoft.VisualBasic.ChrW(10) & "      (n: terminos, vi: base in" &
    "icial, r: valor de x, arg: denominador)"
        '
        'Form1
        '
        Me.AutoScaleDimensions = New System.Drawing.SizeF(9.0!, 21.0!)
        Me.AutoScaleMode = System.Windows.Forms.AutoScaleMode.Font
        Me.AutoSize = True
        Me.BackColor = System.Drawing.Color.White
        Me.ClientSize = New System.Drawing.Size(857, 665)
        Me.Controls.Add(Me.Label1)
        Me.Controls.Add(Me.Results2)
        Me.Controls.Add(Me.Results)
        Me.Controls.Add(Me.Label17)
        Me.Controls.Add(Me.Label15)
        Me.Controls.Add(Me.Label16)
        Me.Controls.Add(Me.Label14)
        Me.Controls.Add(Me.Label13)
        Me.Controls.Add(Me.TextBox4)
        Me.Controls.Add(Me.Label12)
        Me.Controls.Add(Me.Label11)
        Me.Controls.Add(Me.Label10)
        Me.Controls.Add(Me.Label9)
        Me.Controls.Add(Me.Label8)
        Me.Controls.Add(Me.Label7)
        Me.Controls.Add(Me.Label6)
        Me.Controls.Add(Me.Label5)
        Me.Controls.Add(Me.Label4)
        Me.Controls.Add(Me.Button1)
        Me.Controls.Add(Me.Label3)
        Me.Controls.Add(Me.Label2)
        Me.Controls.Add(Me.TextBox3)
        Me.Controls.Add(Me.TextBox2)
        Me.Controls.Add(Me.TextBox1)
        Me.Controls.Add(Me.MenuStrip1)
        Me.Font = New System.Drawing.Font("Segoe UI", 12.0!, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point)
        Me.MainMenuStrip = Me.MenuStrip1
        Me.Margin = New System.Windows.Forms.Padding(4)
        Me.Name = "Form1"
        Me.StartPosition = System.Windows.Forms.FormStartPosition.CenterScreen
        Me.Text = "Práctico - Univ. Luis Gabriel Janco Alvarez"
        Me.MenuStrip1.ResumeLayout(False)
        Me.MenuStrip1.PerformLayout()
        Me.ResumeLayout(False)
        Me.PerformLayout()

    End Sub

    Friend WithEvents Label1 As Label
    Friend WithEvents MenuStrip1 As MenuStrip
    Friend WithEvents OperacionesToolStripMenuItem As ToolStripMenuItem
    Friend WithEvents MultiplicarToolStripMenuItem As ToolStripMenuItem
    Friend WithEvents DivisionToolStripMenuItem As ToolStripMenuItem
    Friend WithEvents SumaToolStripMenuItem As ToolStripMenuItem
    Friend WithEvents RestaToolStripMenuItem As ToolStripMenuItem
    Friend WithEvents TextBox1 As TextBox
    Friend WithEvents TextBox2 As TextBox
    Friend WithEvents TextBox3 As TextBox
    Friend WithEvents Results As TextBox
    Friend WithEvents SeriesToolStripMenuItem As ToolStripMenuItem
    Friend WithEvents SerieRegularToolStripMenuItem As ToolStripMenuItem
    Friend WithEvents Button1 As Button
    Friend WithEvents SerieLogaritmoToolStripMenuItem As ToolStripMenuItem
    Friend WithEvents Results2 As TextBox
    Friend WithEvents SerieProgresivaYRegresivaToolStripMenuItem As ToolStripMenuItem
    Friend WithEvents Label3 As Label
    Friend WithEvents Label2 As Label
    Friend WithEvents Label4 As Label
    Friend WithEvents Label5 As Label
    Friend WithEvents SerieConFactorialToolStripMenuItem As ToolStripMenuItem
    Friend WithEvents Label6 As Label
    Friend WithEvents Label7 As Label
    Friend WithEvents Label8 As Label
    Friend WithEvents Label9 As Label
    Friend WithEvents SerieToolStripMenuItem As ToolStripMenuItem
    Friend WithEvents Label10 As Label
    Friend WithEvents SerieProgresivaConFibonacciToolStripMenuItem As ToolStripMenuItem
    Friend WithEvents Label11 As Label
    Friend WithEvents SerieRegularPinponearToolStripMenuItem As ToolStripMenuItem
    Friend WithEvents Label12 As Label
    Friend WithEvents Label13 As Label
    Friend WithEvents TextBox4 As TextBox
    Friend WithEvents SerieAcumulativaPinponeaToolStripMenuItem As ToolStripMenuItem
    Friend WithEvents Label14 As Label
    Friend WithEvents Label16 As Label
    Friend WithEvents ToolStripMenuItem2 As ToolStripMenuItem
    Friend WithEvents SerieToolStripMenuItem1 As ToolStripMenuItem
    Friend WithEvents Label15 As Label
    Friend WithEvents SerieBaseVaDoblandoToolStripMenuItem As ToolStripMenuItem
    Friend WithEvents Label17 As Label
    Friend WithEvents ParcialToolStripMenuItem As ToolStripMenuItem
    Friend WithEvents AcumularTerminoToolStripMenuItem As ToolStripMenuItem
End Class

 ```
