This solution demonstrates an issue I see with Visual Studio 2017 (15.4.4) and
the Azure Functions SDK NuGet package. Unit tests inside new .csproj projects that
depend on that package don't show up in the Test Explorer. Maybe unit test discovery
is somehow overridden by the Functions SDK or one of its dependencies?

Just build the solution and only the VisibleTestMethod() inside UnitTestProject2
will be shown in the Test Explorer window.