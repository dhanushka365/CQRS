# create the project the Core Layer
- cd CQRS-ES
- dotnet new classlib -o CQRS.Core

# create the project Solution file
- cd SM-POST
- dotnet new sln

# create the project APi Layer for Post Command Project
- cd SM-POST
- cd Post.Cmd
- dotnet new webapi -o Post.Cmd.Api

# create the projet Domain Layer for Post Command Project
- cd SM-POST
- cd Post.Cmd
- dotnet new classlib -o Post.Cmd.Domain


# create the project APi Layer for Post Query Project
- cd SM-POST
- cd Post.Query
- dotnet new webapi -o Post.Query.Api

# create the project Domain Layer for Post Query Project
- cd SM-POST
- cd Post.Query
- dotnet new classlib -o Post.Query.Domain


