# BuildError

## Source code
```
namespace BuildError
{
    class Program
    {
        static void Main()
        {
            MissingType myVar;
        }
    }
}
```

## Visual Studio 2015 (14.0.25420.1)
### Command line :
"C:\Program Files (x86)\Microsoft Visual Studio 14.0\Common7\IDE\devenv.com" "C:\BuildError\BuildError.csproj" /Build Release
### Output :
```
Microsoft Visual Studio 2015 Version 14.0.25420.1.
Copyright (C) Microsoft Corp. All rights reserved.
1>------ Build started: Project: BuildError, Configuration: Release Any CPU ------
1>C:\BuildError\Program.cs(8,13,8,24): error CS0246: The type or namespace name 'MissingType' could not be found (are you missing a using directive or an assembly reference?)
1>C:\BuildError\Program.cs(8,25,8,30): warning CS0168: The variable 'myVar' is declared but never used
========== Build: 0 succeeded, 1 failed, 0 up-to-date, 0 skipped ==========
```

## Visual Studio 2019 (16.7.2)
### Command line :
"C:\Program Files (x86)\Microsoft Visual Studio\2019\Professional\Common7\IDE\devenv.com" "C:\BuildError\BuildError.csproj" /Build Release 
### Output :
```
Microsoft Visual Studio 2019 Version 16.7.2.
Copyright (C) Microsoft Corp. All rights reserved.
1>------ Build started: Project: BuildError, Configuration: Release Any CPU ------
========== Build: 0 succeeded, 1 failed, 0 up-to-date, 0 skipped ==========
```
