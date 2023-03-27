# NETCoreRestfulMongoDBAtlas

## Projeto

Projeto simples criando uma API C# restful e utilizando MongoDB Atlas.

## Projeto utiliza
- Ubuntu 22.04.2 LTS
- vscode
- C#
- MongoDB Atlas

## Pré-requisitos
#  Iniciar C#

Caso usar ctrl-c + ctrl-v
Dentro da pasta do projeto
```
dotnet new webapi
dotnet add package MongoDB.Driver
dotnet add package mongocsharpdriver
dotnet add NAME_YOUR_FILE.csproj package Swashbuckle.AspNetCore
```

# Adicionar
appsettings.json

´´´

{
    ...
    
    "Logging": {
        "LogLevel": {
            "Default": "Information",
            "Microsoft.AspNetCore": "Warning"
        }
    },
    "AllowedHosts": "*",
    "MongoDB": {
        "ConnectionURI": "ATLAS_URI_HERE",
        "DatabaseName": "sample_mflix",
        "CollectionName": "playlist"
    }

    ....
}


´´´

# Criar uma base de dados
- Database name: sample_mflix
- Collection Name:  playlist

# Rodar o projeto

```
dotnet run
```

# Documentação do swagger

- https://localhost:PORT/swagger