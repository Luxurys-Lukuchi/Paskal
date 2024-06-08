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
