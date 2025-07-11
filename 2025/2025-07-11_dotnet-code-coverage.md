# 2025-07-11 - .NET Code Coverage

I always forget the commands to run code coverage and generate reports from the CLI (locally).

Generally it's configured on a build server for Continuous Integration, but often I just want to run it locally.
I also tend to just use Rider, which has it built in, but sometimes it doesn't work fully (not sure why).

So this post is a little reminder for me, so I don't have to go searching the docs :)

For report generation, there's the dotnet tool:

```shell
$ dotnet tool install -g dotnet-reportgenerator-globaltool
```

To run the code coverage:

```shell
$ dotnet test --collect:"XPlat Code Coverage"
```

This will generate reports in a format for other tooling, and then the report generator can generate HTML from this:

```shell
$ reportgenerator -reports:"**/coverage.cobertura.xml" -targetdir:"coverage" -reporttypes:Html
```
