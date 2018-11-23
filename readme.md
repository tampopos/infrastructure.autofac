# tmpps.infrastructure.autofac

## register nuget

```bash
npm run publish
# replace version,api-key
dotnet nuget push ./Tmpps.Infrastructure.Autofac/bin/Release/Tmpps.Infrastructure.Autofac.${version}.nupkg -k ${api-key} -s https://api.nuget.org/v3/index.json
```
