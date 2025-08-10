`dotnet build .\library`

`dotnet pack .\library`

`dotnet nuget locals all -c`

`dotnet add .\application\ package library --source .\library\bin\Release\`

`dotnet restore .\application\`

`dotnet  run  -p  .\application\`

`dotnet build .\otherlibrary`

`dotnet pack .\otherlibrary\`

`dotnet nuget locals all -l`

Replace library nuget and .dll in global cache

`dotnet restore .\application\  --locked-mode`

`dotnet run --project .\application\`