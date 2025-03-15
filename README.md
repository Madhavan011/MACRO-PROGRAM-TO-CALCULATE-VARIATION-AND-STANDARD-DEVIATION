# MACRO-PROGRAM-TO-CALCULATE-VARIATION-AND-STANDARD-DEVIATION
Sub varandstd()

Dim dataRange As Range

Dim variation As Double

Dim stdDev As Double 

Set dataRange = ActiveSheet.Range("A2:A100") 

variation = WorksheetFunction.Var(dataRange)

stdDev = WorksheetFunction.StDev(dataRange) 

MsgBox "Variation: " & variation & vbCrLf & "Standard Deviation: " & stdDev

End Sub
