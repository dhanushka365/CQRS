# create the project the Core Layer
- cd CQRS-ES
- dotnet new classlib -o CQRS.Core

# create the project Solution file
- cd SM-POST
- dotnet new sln

# create the project APi Layer for Post.Cmd Microservice
- cd SM-POST
- cd Post.Cmd
- dotnet new webapi -o Post.Cmd.Api

# create the projet Domain Layer for Post.Cmd Microservice
- cd SM-POST
- cd Post.Cmd
- dotnet new classlib -o Post.Cmd.Domain


# craete the Infrastructure Layer for Post.Cmd Microservice
- cd SM-POST
- cd Post.Cmd
- dotnet new classlib -o Post.Cmd.Infrastructure


# create the project APi Layer for Post.Query Microservice
- cd SM-POST
- cd Post.Query
- dotnet new webapi -o Post.Query.Api

# create the project Domain Layer for Post.Query Microservice
- cd SM-POST
- cd Post.Query
- dotnet new classlib -o Post.Query.Domain

# craete the Infrastructure Layer for Post.Query Microservice
- cd SM-POST
- cd Post.Query
- dotnet new classlib -o Post.Query.Infrastructure

# add CQRS.Core projects into solution file
- cd SM-POST
- dotnet sln add ../CQRS-ES/CQRS.Core/CQRS.Core.csproj

# add Post.cmd.APi project into solution file
- cd SM-POST
- dotnet sln add Post.Cmd/Post.Cmd.Api/Post.cmd.Api.csproj

# add Post.cmd.Domain project into solution file
- cd SM-POST
- dotnet sln add Post.Cmd/Post.Cmd.Domain/Post.cmd.Domain.csproj

# add Post.cmd.Infrastructure project into solution file
- cd SM-POST
- dotnet sln add Post.Cmd/Post.Cmd.Infrastructure/Post.cmd.Infrastructure.csproj