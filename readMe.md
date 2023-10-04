# create the Core Layer
- cd CQRS-ES
- dotnet new classlib -o CQRS.Core

# create the project Solution file
- cd SM-POST
- dotnet new sln

# create Post Command Project
- cd SM-POST
- cd Post.Cmd
- dotnet new webapi -o Post.Cmd.Api