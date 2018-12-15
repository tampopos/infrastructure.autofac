# tmpps.infrastructure.autofac

## command

#### build

`dotnet build Tmpps.Infrastructure.Autofac.Tests/`

#### test

`dotnet test Tmpps.Infrastructure.Autofac.Tests/`

#### register nuget

```bash
dotnet build -c Release Tmpps.Infrastructure.Autofac
# replace version,api-key
dotnet pack -c Release --include-source -p:PackageVersion=${version} Tmpps.Infrastructure.Autofac
dotnet nuget push ./Tmpps.Infrastructure.Autofac/bin/Release/Tmpps.Infrastructure.Autofac.${version}.nupkg -k ${api-key} -s https://api.nuget.org/v3/index.json
```

## use circleCI CLI

#### validation config

`circleci config validate`

#### test

`circleci local execute --job test`

#### release

```bash
git tag X.Y.Z
git push origin --tags
```
