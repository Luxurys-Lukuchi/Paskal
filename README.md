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


# Paskal 2
![изображение](https://github.com/Luxurys-Lukuchi/Paskal/assets/146846830/d81c78f7-22c4-451a-af95-50ec59a6a2d6)


program ComputeFunction;

uses

  Math;

var
  
  x, a, y: Real;

begin
  
  // Запросить у пользователя ввод значений для x и a
  
  Write('Введите значение для x: ');
  
  ReadLn(x);
  
  Write('Введите значение для a: ');
  
  ReadLn(a);

  // Вычислить значение y в зависимости от условий
  
  if (x < 2) and (a > 3) then
  
    y := 9.38 * Sin((Power(x, 3) - 7 * a) / Power(a, 3))
  
  else if (x < 2) and (a <= 3) then
  
    y := Ln(Abs(Power(a, 3))) + Cos(x)
  
  else if (x >= 2) then
  
    y := Tan(Sin(x));

  // Вывести результат на экран
  
  WriteLn('Вычисленное значение y = ', y:0:4);

end.

# Pacsal 3
![изображение](https://github.com/Luxurys-Lukuchi/Paskal/assets/146846830/8407578e-7e0a-4d38-bd42-45a2ff377b6d)

program CalculateExpressions;

var

  a, b: Real;
  
  i, k: Integer;

begin
  
  a := 0.0;
  
  b := 1.0;

  // Вычисление значения a
  
  for i := 1 to 7 do
  
    a := a + (i * i / 5);

  // Вычисление значения b
  
  for k := 1 to 5 do
  
    b := b * (1 / k);

  // Вывод результатов на экран
  
  WriteLn('Значение a = ', a:0:4);
  
  WriteLn('Значение b = ', b:0:4);

end.

![изображение](https://github.com/Luxurys-Lukuchi/Paskal/assets/146846830/8bf0b740-3d8a-4408-8735-4d4ed9fd7e45)

program TableUsingWhile;

var
  
  x, y: Real;
  
  h: Real;

begin
  
  h := 2.0;
  
  x := 5.0;

  WriteLn(' x    |    y');
  
  WriteLn('--------------');
  
  
  while x <= 25.0 do
  
  begin
  
    y := Sqrt(5 * x);
    
  WriteLn(x:4:1, ' | ', y:6:4);
  
    x := x + h;
  
  end;

end.

-------------------------------

program TableUsingRepeat;

var
  
  x, y: Real;
  
  h: Real;

begin
  
  h := 2.0;
  
  x := 5.0;

  
  WriteLn(' x    |    y');
  
  WriteLn('--------------');
  
  repeat
  
    y := Sqrt(5 * x);
    
    WriteLn(x:4:1, ' | ', y:6:4);
    
    x := x + h;
  
  until x > 25.0;

end.
