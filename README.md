# Study Jetbrains Rider + Unit Tests

Study case of Jetbrains Rider cross platform .NET IDE using .NET Core + Unit Tests

## Dependencies

- **apt-transport-https**

```sh
sudo apt-get update
sudo apt-get install apt-transport-https
```

- Install JetBrains Rider

- Download and install : https://www.jetbrains.com/rider/download/

- Install .NET Core SDK

```sh
sudo apt-get install dotnet-sdk-3.1
```

- Install ASP.NET Core Runtime

```sh
sudo apt-get install aspnetcore-runtime-3.1
```

- Install .NET Core Runtime

```sh
sudo apt-get update
sudo apt-get install dotnet-runtime-3.1
```

## Steps to reproduce

- Create new Solutions

```sh
dotnet new sln
```

- Create classlib PrimeService

```sh
dotnet new classlib -n PrimeService && cd PrimeService
```

- Rename Class1.cs to PrimeService.cs

```sh
mv Class1.cs PrimeService.cs
```

- Create PrimeService method

```sh
using System;

namespace Prime.Services
{
    public class PrimeService
    {
        public bool IsPrime(int candidate)
        {
            throw new NotImplementedException("Please create a test first.");
        }
    }
}
```

- Inside root of project type the command `dotnet sln add PrimeService/PrimeService.csproj`

## References

- [.NET Core Unit Tests](https://docs.microsoft.com/pt-br/dotnet/core/testing/unit-testing-with-dotnet-test)
- [.NET Core](https://dotnet.microsoft.com/download)
- [.NET Core + Ubuntu](https://docs.microsoft.com/pt-br/dotnet/core/install/linux-package-manager-ubuntu-1904)
