#### dotnet version
- dotnet --version

#### list of all sdk's installed
- dotnet --info

#### dot net help
- dotnet -h

#### dot net project templates (template name, short name, languages and tags)
- dotnet new list

#### create dot net solution file
- dotnet new sln

#### create new project
- dotnet new webapi -controllers -n [API]

#### add project to solution
- dotnet sln add [API]

#### trust certificate
-  sudo dotnet dev-certs https --trust
- if above not working clean first and run above command
- sudo dotnet dev-certs https --clean

#### runs dotnet project
- dotnet run

#### runs dotnet project after changes
- dotnet watch

#### install dotnet ef
- dotnet tool install --global dotnet-ef --version [9.0.0]

#### dotnet tools with version
- dotnet tool list -g

#### dotnet ef information
- dotnet ef

#### dotnet migrations command help
- dotnet ef migrations -h

#### add new migrations
- dotnet ef migrations add [InitialCreate] -o [Data/Migrations]
- dotnet ef migrations add [UserEntityUpdated]

#### to undo newly created migrations
- dotnet ef migrations remove

#### database info
- dotnet ef database -h

#### Updates the database to a specified migration.
-- dotnet ef database update

#### add dotnet gitignone file
- dotnet new gitignore

#### quick fix/ show code actions
- command + .
