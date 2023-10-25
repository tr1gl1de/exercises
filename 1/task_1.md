## Задача 1
Написать консольное приложение для поиска слова с наибольшим кол-вом гласных.
В качестве аргумента передать путь до файла

### Пример вызова готового приложения
В директории приложения (условно C:\my-console-app\) вызывать комманду ниже
> через PowerShell `dotnet run --"C:\\my-console-app\new-folder\file-with-text.txt"`

Почитать про CLI dotnet (по сути для работы через консоль с dotnet) можно [тут][dotnet-tool-link]

### Советы
Для получения аргументов командной строки можно использовать данный код
```C#
string name = Environment.GetCommandLineArgs()[1];
// или
string newName = Environment.GetCommandLineArgs().First();
```
так же по правилам хорошего тона, вместо указания типа в примере выше (это `string`) лучше использовать `var`
```C#
var name = Environment.GetCommandLineArgs()[1];
// или
var newName = Environment.GetCommandLineArgs().First();
```


[dotnet-tool-link]: https://learn.microsoft.com/ru-ru/dotnet/core/tools/dotnet