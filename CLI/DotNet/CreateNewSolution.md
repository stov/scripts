- Create the solution
- Create 2 new console projects
- Add projects to the solution
- Build the solution (all projects)
```
dotnet new sln --name FooBar
dotnet new console --name Foo --output Foo
dotnet new console --name Bar --output Bar
dotnet sln add .\Foo\Foo.csproj
dotnet sln add .\Bar\Bar.csproj
dotnet restore
dotnet build FooBar.sln
```

Run from csproj file
```
cd Foo
dotnet run
```

Run from dll
```
cd bin\debug\netcoreapp2.0
dotnet Foo.dll
```
