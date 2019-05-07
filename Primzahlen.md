
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


Public Function Primzahl(ByVal Prim As Long) As Boolean
    Dim i As Long                        
    For i = 2 To Prim - 1                
        If Prim Mod i = 0 Then           
            Primzahl = False             
            Exit Function                
        End If                           
    Next I                            
    Primzahl = True
End Function

end module
