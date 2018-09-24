# Microservice.PoC.Steeltoe

## Steeltoe

[![N|Steeltoe](https://www.cnblogs.com/images/cnblogs_com/edisonchou/1260867/o_logo-banner.PNG)](http://steeltoe.io/)<br/>
Steeltoe is an open source project that enables .NET developers to implement industry standard best practices when building resilient microservices for the cloud. The Steeltoe client libraries enable .NET Core and .NET Framework apps to easily leverage Netflix Eureka, Hystrix, Spring Cloud Config Server, and Cloud Foundry services.<br/>
For more details, please read this => http://steeltoe.io/<br/>
What's more, Pivotal provide a sample application on Github => https://github.com/SteeltoeOSS/Samples/tree/master

Steeltoe enable .NET/.NET Core to use the below components at this moment:
  - Service Discovery
  - Config Server
  - Circuit Breaker
  - Cloud Connectors

## About this sample

[![N|ASP.NET Core](https://www.cnblogs.com/images/cnblogs_com/edisonchou/1260867/o_aspnet-core-logo.PNG)](https://docs.microsoft.com/zh-cn/aspnet/core/getting-started/?view=aspnetcore-2.1&tabs=windows)<br/>
This sample is a microservice project developed by ASP.Net Core with Spring Cloud based on Steeltoe, it integrated with the below Spring Cloud components:
  - Eureka : [Java-EurekaServer](https://github.com/Manulife-Chengdu/Microservice.PoC.Steeltoe/tree/master/springcloud/eureka-service), [Chapter1-ServiceDiscovery](https://github.com/Manulife-Chengdu/Microservice.PoC.Steeltoe/tree/master/src/Chapter1-ServiceDiscovery)
  - Zuul : [Java-ZuulServer](https://github.com/Manulife-Chengdu/Microservice.PoC.Steeltoe/tree/master/springcloud/zuul-service), [Chapter1-ServiceDiscovery](https://github.com/Manulife-Chengdu/Microservice.PoC.Steeltoe/tree/master/src/Chapter1-ServiceDiscovery)
  - Hystrix : [Java-Dashboard](https://github.com/Manulife-Chengdu/Microservice.PoC.Steeltoe/tree/master/springcloud/hystrix-dashboard-service), [Chapter2-CircuitBreaker](https://github.com/Manulife-Chengdu/Microservice.PoC.Steeltoe/tree/master/src/Chapter2-CircuitBreaker)
  - Config Server : 

## Installation

To use Steeltoe in .Net Core, we can use the below NuGet packages:<br/>
Service Discovery Client
```sh
PM> Install-Package Pivotal.Discovery.ClientCore
```
Circuit Breaker Core
```sh
PM> Install-Package Steeltoe.CircuitBreaker.HystrixCore
```
Hystrix Metrics
```sh
PM> Install-Package Steeltoe.CircuitBreaker.Hystrix.MetricsEventsCore
```


## Rerference

  - [.NET Core微服务之基于Steeltoe使用Spring Cloud Eureka实现服务注册与发现](https://www.cnblogs.com/edisonchou/p/dotnet_core_microservice_integrate_with_springcloud_eureka.html)
  - [.NET Core微服务之基于Steeltoe集成Spring Cloud Zuul实现统一API网关](https://www.cnblogs.com/edisonchou/p/dotnet_core_microservice_integrate_with_springcloud_zuul.html)
  - [.NET Core微服务之基于Steeltoe集成Spring Cloud Hystrix实现熔断保护与可视化监控](https://www.cnblogs.com/edisonchou/p/dotnet_core_microservice_integrate_with_springcloud_hystrix.html)