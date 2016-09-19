# lucky
var
    i: integer;

begin
    for i := 100 to 999 do 
        if (i mod 10 = (i div 10) mod 10 + i div 100) or (i div 100 = i mod 10 + (i div 10) mod 10) then
            if ((i + 1) mod 10 = ((i + 1) div 10) mod 10 + (i + 1) div 100) or ((i + 1) div 100 = (i + 1) mod 10 + ((i + 1) div 10) mod 10) then
            begin
                writeln(i);
                break;
            end;
end.
