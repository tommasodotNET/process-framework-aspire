# Process Framework with .NET Aspire

This demo aims to showcase how the [Semantic Kernel Process Framework](https://learn.microsoft.com/en-us/semantic-kernel/overview/) can be used with [.NET Aspire](https://learn.microsoft.com/en-us/dotnet/aspire/get-started/aspire-overview). The Process Framework allows developers to create business processes based on events. Each step of the process can be an agent or native code.

In this demo, I have defined the agents as external services, and each step will call these agents using HTTP requests. This setup allows .NET Aspire to add value by tracing the process using OpenTelemetry. Additionally, since each agent is a service, they can be restarted as needed using the .NET Aspire developer dashboard.
