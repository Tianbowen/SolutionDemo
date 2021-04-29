# SolutionDemo
Build ASP.NET Core 3.1 production-ready solution from the ground up

src – solution source files which includes all projects sources

docs – documentation on your solution. This could be any diagrams which contains sequence or activity flows or just a simple use cases

tests – all kind of tests for your solution including unit tests, integration tests, acceptance tests, etc.

build – could be any scripts for building your solution

deploy – scripts related to deploying your solution to different environments or localhost

.gitattributes – Defines Git behavior on certain attributes-aware operations like line endings, merge settings for different file types and much more.

.gitignore – Defines patterns for files which should be ignored by Git (like binaries, tooling output, etc). This one adapted for Visual Studio/Code and .NET projects

.gitlab-ci.yml – Configuration file for GitLab pipeline (will be covered in Part 2). We would like to be sure that our code continuously integrated and delivered.

README.md – Every well-made project should contain readme file with instructions on how to build and run your solution, optionally, with team members and responsible persons.

Directory.Build.props is a user-defined file that provides customizations to projects under a directory.

When MSBuild runs, Microsoft.Common.props searches your directory structure for the Directory.Build.props file (and Microsoft.Common.targets looks for Directory.Build.targets). If it finds one, it imports the property.

dotnet add package SonarAnalyzer.CSharp
dotnet add package SecurityCodeScan
dotnet add package StyleCop.Analyzers

dotnet tool install -g dotnet-format
	
dotnet format
