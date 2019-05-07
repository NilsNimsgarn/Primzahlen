
module main

sub main()
dim ergebnis as string
dim nummer as integer

nummer=console.readline()
for x as integer=2 to nummer

if primzahl(x)=true then
ergebnis=ergebnis & x.tostring & " "
end if

next
console.writeline(ergebnis)
console.readline()
end sub


Public Function Primzahl(ByVal Prim As Long) As Boolean    ' Die Funktion liefert einen
    Dim i As Long                        ' Booleschen Wert zurück. Der 
    For i = 2 To Prim - 1                    ' Parameter Prim bildet die Basis 
        If Prim Mod i = 0 Then                    ' der Funktion. Ansonsten gilt die
            Primzahl = False                    ' Struktur der alten j- Schleife.
            Exit Function                        ' Prim stellt die zu testende 
        End If                            ' Primzahl dar, was aber klar sein
    Next I                            ' sollte.
    Primzahl = True
End Function

end module
