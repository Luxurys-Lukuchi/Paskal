# Paskal 1
![изображение](https://github.com/Luxurys-Lukuchi/Paskal/assets/146846830/669bb722-2514-48fc-ab78-565341107461)

program N1;

uses
  
  Math;

var
  
  x, a, b, t, y, Z: Real;

begin

  // Запросить у пользователя ввод значений для x, a и b

  Write('Введите значение для x: ');
  
  ReadLn(x);
  
  Write('Введите значение для a: ');
  
  ReadLn(a);
  
  Write('Введите значение для b: ');
  
  ReadLn(b);

  // Вычислить значение t
  
  t := (Tan(a / b)) / (x * x + 5.7);

  // Вычислить значение y
  
  y := Abs(t) - Sin(Cos(a));

  // Вычислить значение Z
  
  Z := Exp(-t) + Power(t, 4);

  // Вывести результаты на экран
  
  WriteLn('Вычисленные значения:');
  
  WriteLn('t = ', t:0:4);
  
  WriteLn('y = ', y:0:4);
  
  WriteLn('Z = ', Z:0:4);

end.
