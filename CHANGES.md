1.2.0, 1.2.0.{dw9, dw8, dw7} :: Oct. 12, 2017
---
* [Dropwizard 1.2.0](https://github.com/dropwizard/dropwizard/releases/tag/v1.2.0)
* Mockito-core 2.10.0
* Merged a PR converting to a lot of [Java8](https://github.com/yammer/tenacity/pull/44) equivalents

1.1.4, 1.1.4.{dw9, dw8, dw7} :: Aug. 7, 2017
---
* [Dropwizard 1.1.3](https://github.com/dropwizard/dropwizard/releases/tag/v1.1.3)
* `waitForInitialLoad` blocks an application from starting until Breakerbox configurations are fetched.
* Fixing `hystrix-metrics-event-stream` from pulling in an older version of servlet-api

1.1.3, 1.1.3.{dw9, dw8, dw7} :: July 13, 2017
---
* [Hystrix 1.5.13](https://github.com/Netflix/Hystrix/blob/master/CHANGELOG.md#version-1513-maven-central-bintray)
* [Dropwizard 1.1.2](https://github.com/dropwizard/dropwizard/releases/tag/v1.1.2)
* Assertj-core 3.8.0
* Mockito-core 2.8.47
* Error_prone_core 2.0.21
* Adding jcenter/bintray repository

1.1.2, 1.1.2.{dw9, dw8, dw7} :: May. 19, 2017
---
* [Hystrix 1.5.12](https://github.com/Netflix/Hystrix/blob/master/CHANGELOG.md#version-1512-maven-central-bintray)
* [Dropwizard 1.1.1](https://github.com/dropwizard/dropwizard/releases/tag/v1.1.1)

1.1.1, 1.1.1.{dw9, dw8, dw7} :: Apr. 11, 2017
---
* [Hystrix 1.5.11](https://github.com/Netflix/Hystrix/blob/master/CHANGELOG.md#version-1511-maven-central-bintray)
* [COMMAND_MAX_ACTIVE issue](https://github.com/Netflix/Hystrix/pull/1513)

1.1.0, 1.1.0.{dw9, dw8, dw7} :: Mar. 21, 2017
---
* [Hystrix 1.5.10](https://github.com/Netflix/Hystrix/blob/master/CHANGELOG.md#version-1510-maven-central-bintray)
* [Dropwizard 1.1.0](http://www.dropwizard.io/1.1.0/docs/about/release-notes.html#v1-1-0-mar-21-2017)

1.0.5, 1.0.5.{dw9, dw8, dw7} :: Dec. 21, 2016
---
* [Hystrix 1.5.9](https://github.com/Netflix/Hystrix/blob/master/CHANGELOG.md#version-159-maven-central-bintray)
* [Dropwizard 1.0.5](http://www.dropwizard.io/1.0.5/docs/about/release-notes.html)
* Added [Google Error-Prone](https://github.com/google/error-prone) to the build

1.0.4, 1.0.4.{dw9, dw8, dw7} :: Nov. 6, 2016
---
* `TenacityConfiguredBundle` won't initialize if another `HystrixMetricsPublisher` is registered. This is usually encountered when
   you try to run multiple `DropwizardAppRule` instances within a given test. Relaxing this constraint to just log a warning and to
   display the currently registered `HystrixMetricsPublisher` instead of preventing startup.
* [Hystrix 1.5.7](https://github.com/Netflix/Hystrix/blob/master/CHANGELOG.md#version-157-maven-central-bintray)
* [Dropwizard 1.0.3](http://www.dropwizard.io/1.0.3/docs/about/release-notes.html)
* Assertj-guava 3.1.0

1.0.3, 1.0.3.{dw9, dw8, dw7} :: Oct. 10, 2016
---
* Tenacity `ExceptionMapper`s no longer throw exceptions anymore when they don't match a specific requirement. They should always
resolve the exception gracefully into a `Response`.

1.0.2, 1.0.2.{dw9, dw8, dw7} :: Sept. 28, 2016
---
* [Hystrix 1.5.6](https://github.com/Netflix/Hystrix/blob/master/CHANGELOG.md#version-156-maven-central-bintray)
* [Dropwizard 1.0.2](http://www.dropwizard.io/1.0.2/docs/about/release-notes.html#v1-0-2-sep-23-2016)

1.0.1, 1.0.1.{dw9, dw8, dw7} :: August 8, 2016
---
* [Hystrix 1.5.4](https://github.com/Netflix/Hystrix/blob/master/CHANGELOG.md#version-154-maven-central-bintray)
* Fixing bug for TenacityCommand/TenacityObservableCommand builders generics. They take two parameters for an expectant Function<T, R> but it actually only ever uses Supplier<R> so the first parameter is completely useless. Removing it entirely.
* `TenacityTestRule` has additional stream-related resets.

1.0.0 :: July 26, 2016
---
* [Dropwizard 1.0.0](https://dropwizard.io/1.0.0/docs)
* Java8
* `TenacityCommand` and `TenacityObservableCommmand` now have fluent builders that leverage functional interfaces for command construction
* No planned releases for dw7, dw8, dw9 since this is largely a Dropwizard 1.0.0 release.

0.8.3, 0.8.3-dw8, 0.8.3-dw7 :: June 10, 2016
---
* [Hystrix 1.5.3](https://github.com/Netflix/Hystrix/blob/master/CHANGELOG.md#version-153-maven-central-bintray)

0.8.2, 0.8.2-dw8, 0.8.2-dw7 :: Apr 14, 2016
---
* Removing calculating `latencyTotal_percentile_98` and `latencyExecute_percentile_98` as they are no longer available in HystrixCommands

0.8.1, 0.8.1-dw8, 0.8.1-dw7 :: Apr 14, 2016
---
* [Hystrix 1.5.2](https://github.com/Netflix/Hystrix/blob/master/CHANGELOG.md#version-152-maven-central-bintray)
* AssertJ Core 2.4.1
* TenacityCommand now accepts a `TenacityPropertyKey` if you want to control which threadpool is associated with your command
* [Type parameter names should comply with a naming conversion PR #34](https://github.com/yammer/tenacity/pull/34)
* [Multiple code improvements PR #33](https://github.com/yammer/tenacity/pull/33)

0.8.0, 0.8.0-dw8, 0.8.0-dw7 :: Mar 10, 2016
---
* [Hystrix 1.5.1](https://github.com/Netflix/Hystrix/blob/master/CHANGELOG.md#version-151-maven-central-bintray)
* Tenacity Bill of Materials (tenacity-bom for dependencyManagement)
* AssertJ Core 2.3.0
* AssertJ Guava 2.0.0

0.7.3, 0.7.3-dw8, 0.7.3-dw7 :: Jan 21, 2016
---
* [Hystrix 1.4.23](https://github.com/Netflix/Hystrix/blob/master/CHANGELOG.md#version-1423-maven-central-bintray)
* Dropwizard 0.9.2
* New version release strategy. Hopefully it is clearer that 0.7.3 is the latest dropwizard version (0.9.x) while 0.7.3-dw8 supports legacy dropwizard-0.8.5, and 0.7.3-dw7 supports legacy dropwizard 0.7.1

Dropwizard 0.9.x releases
=========================
0.7.2 - Nov 23, 2015
---
* [Hystrix 1.4.21](https://github.com/Netflix/Hystrix/blob/master/CHANGELOG.md#version-1421-maven-central-bintray)

0.7.1 - Nov 16, 2015
---
* [Hystrix 1.4.20](https://github.com/Netflix/Hystrix/blob/master/CHANGELOG.md#version-1420-maven-central-bintray)
* Findbugs 3.0.3

0.7.0 - Nov 5, 2015
---
* Dropwizard 0.9.1
* Findbugs 3.0.2
* Upgraded maven-*-plugins

Dropwizard 0.8.x releases
=========================
0.6.19 - Nov 23, 2015
---
* Backport of 0.7.2

0.6.18 - Nov 16, 2015
---
* Backport of 0.7.1
* Dropwizard 0.8.5

0.6.17
---
* [Hystrix 1.4.18](https://github.com/Netflix/Hystrix/blob/master/CHANGELOG.md#version-1418-maven-central-bintray)

0.6.16
---
* [Hystrix 1.4.17](https://github.com/Netflix/Hystrix/blob/master/CHANGELOG.md#version-1417-maven-central-bintray)
* RxJava 1.0.14

0.6.15
---
* [Hystrix 1.4.16](https://github.com/Netflix/Hystrix/blob/master/CHANGELOG.md#version-1416-maven-central-bintray)

0.6.14
----
* [Hystrix 1.4.15](https://github.com/Netflix/Hystrix/blob/master/CHANGELOG.md#version-1415-maven-central-bintray)
* Ability to move /tenacity resources to the admin port. This is tunable by using `usingAdminPort()` when building the `Tenacity` bundle.

0.6.13
----
* Dropwizard 0.8.4
* Removing `ForkedJerseyClientBuilder` since [Dropwizard PR 1137](https://github.com/dropwizard/dropwizard/pull/1137) has been merged into 0.8.2
* Removing deprecated `ClientException` and `ClientResponseResult`

0.6.12
----
* `TenacityObservables` to help with executing two observables. Intended to help execute the first argument eagerly and only
  execute (lazily) the second argument if the primary fails.
* When registering `TenacityConfiguration`s with `Archaius` no longer set the `executionIsolationStrategy` properties, unless
  specifically set by the user.
  This was leading to misconfigurations when using `TenacityObservableCommand`s that default to `SEMAPHORE` isolation.
  This is due to the disconnect between not knowing if a `TenacityConfiguration` is paired with a command that is intended to be used
  as `THREAD` or `SEMAPHORE` isolation prior.
  A user must now explicitly set this within the `TenacityConfiguration` or via `Breakerbox` otherwise it takes the default of the
  command type.

0.6.11
----
* When registering configuration properties with `Archaius` use its hierarchical system so that multiple clients of `Archaius` can register their configurations as well. 
  This changes the behavior from before where `Tenacity` would install a custom configuration different than the sharable default.
* [Hystrix 1.4.14](https://github.com/Netflix/Hystrix/blob/master/CHANGELOG.md#version-1413-maven-central-bintray)

0.6.10
----
* Deprecating `ClientResponseResult` and `ClientException`. These will be removed in the following release. There will be a replacement for this pattern.
* Fixing `DefaultServerFactory` cast in the `TenacityConfigureBundle` [Pull Request #26](https://github.com/yammer/tenacity/pull/26)
* [Hystrix 1.4.13](https://github.com/Netflix/Hystrix/blob/master/CHANGELOG.md#version-1413-maven-central-bintray)
* RxJava 1.0.13

0.6.9
----
* [Hystrix 1.4.12](https://github.com/Netflix/Hystrix/blob/master/CHANGELOG.md#version-1412-maven-central-bintray)

0.6.8
----
* [Hystrix 1.4.11](https://github.com/Netflix/Hystrix/blob/master/CHANGELOG.md#version-1411-maven-central-bintray)
* RxJava 1.0.12

0.6.7
----
* [Hystrix 1.4.10](https://github.com/Netflix/Hystrix/blob/master/CHANGELOG.md#version-1410-maven-central-bintray)
* Hystrix fixing a memory leak that was released in 1.4.8+. This affects Tenacity version 0.6.6.

0.6.6 _MEMORY LEAK fixed in 0.6.7_
-----
* [Hystrix 1.4.9](https://github.com/Netflix/Hystrix/blob/master/CHANGELOG.md#version-149-maven-central-bintray)
* Exclude the transitive dependency on io.dropwizard.metrics.metrics-core 3.1.2

0.6.5
-----
* [Hystrix 1.4.7](https://github.com/Netflix/Hystrix/blob/master/CHANGELOG.md#version-147-maven-central-bintray)
* RxJava 1.0.10

0.6.4
-----
* [Hystrix 1.4.5](https://github.com/Netflix/Hystrix/blob/master/CHANGELOG.md#version-145-maven-central-bintray)
* Added `GET /tenacity/circuitbreaker/{key}`
* Added `PUT /tenacity/circuitbreaker/{key}`. Accepted bodies are `FORCED_CLOSED`, `FORCED_OPEN`, and `FORCED_RESET`.
  This allows specific control over a particular circuit breaker. `FORCED_RESET` returns the circuitbreaker to it's original state
  whether it's neither `FORCED_OPEN` or `FORCED_CLOSED`.
* Added `TenacityCircuitBreakerHealthCheck` which can be enabled via the `TenacityBundleBuilder`. This fails the `/healthcheck`
  when any circuitbreaker is in an open state or not accepting requests.

0.6.3
-----
* Fixed a memory-leak when using `TenacityJerseyClient`. It was incorrectly adjusting the timeout for the shared configuration for all WebTargets created from a parent `JerseyClient` instead of 
  on the per-request configuration that is generated for each invocation of a `WebTarget`. This will be sent to Dropwizard as a pull-request, but for now we have a workaround. You need to create your
  `JerseyClient` using the `ForkedJerseyClientBuilder` instead of Dropwizard's `JerseyClientBuilder`. Note: this is only necessary when using dropwizard 0.8.0 and 0.8.1
* Migrated `WebTarget` out of a jersey related namespace. No use of non-public APIs anymore.
* No backport for this release as it only affects dropwizard 0.8.x


0.6.2
-----
* Fixing bug where `TenacityPropertyStore` wouldn't properly update the `executionIsolationStrategy` to reflect the live configuration value. This only affects Breakerbox's ability to determine
  if configurations are synchronized or not.
* There is a memory-leak when using `TenacityJerseyClient` and Dropwizard <= 0.8.1. Please avoid using `TenacityJerseyClient` in this release.

0.6.1
-----
* Remove `ManagedConcurrencyStrategy` and revert back to the default. This is replicated through `ManagedHystrix`. 
  Hystrix also enforces stricter use of `HystrixRequestContext` semantics when using a custom strategy. This broke use of per-request
  features of Hystrix.
* There is a memory-leak when using `TenacityJerseyClient` and Dropwizard <= 0.8.1. Please avoid using `TenacityJerseyClient` in this release.

0.6.0
-----
* Dropwizard 0.8.1 - This was blocked by [Dropwizard 0.8.0 pull-request](https://github.com/dropwizard/dropwizard/pull/939)
* There is a memory-leak when using `TenacityJerseyClient` and Dropwizard <= 0.8.1. Please avoid using `TenacityJerseyClient` in this release.


Dropwizard 0.7.x Releases
=========================
0.5.22 - Nov 23, 2015
---
* Backport of 0.7.2

0.5.21 - Nov 16, 2015
----
* Backport of 0.7.1

0.5.20
-----
* Backport of 0.6.17

0.5.19
-----
* Backport of 0.6.16

0.5.18
-----
* Backport of 0.6.15

0.5.17
-----
* Backport of 0.6.14
* Jersey 1.x incompatiblities and DW7 not allowing empty JerseyContextes

0.5.16
-----
* Backport of 0.6.13

0.5.15
-----
* Backport of 0.6.12

0.5.14
-----
* Backport of 0.6.11

0.5.13
-----
* Backport of 0.6.10

0.5.12
-----
* Backport of 0.6.9

0.5.11
-----
* Backport of 0.6.8

0.5.10
-----
* Backport of 0.6.7. Fixing a memory leak in 0.5.9.

0.5.9 _MEMORY LEAK fixed in 0.5.10_
-----
* Backport of 0.6.6

0.5.8
----
* Backport of 0.6.5

0.5.7
----
* Backport of 0.6.4 (0.6.3 was a Dropwizard 0.8.1 fix only)

0.5.6
-----
* Backport of 0.6.2

0.5.5
-----
* Backport of 0.6.1

0.5.4
--------------
* [Hystrix 1.4.4](https://github.com/Netflix/Hystrix/blob/master/CHANGELOG.md#version-144-maven-central-bintray)
* `executionIsolationStrategy` is now a configurable through `TenacityConfiguration`. Defaults to `THREAD` isolation. You'd want to normally
  set this to `SEMAPHORE` when using `TenacityObservableCommand`.
  [Breakerbox](https://github.com/yammer/breakerbox) will have a respective update which will also allow you set the `executionIsolationStrategy`.
* Fixing bug where the `TenacityPropertyRegister` would rely on the `toString()` method of the TenacityPropertyKey instead of `name()`.

0.5.3
--------------
* Added `SemaphoreConfiguration`. This enables the ability to configure semaphore specific parameters for when dealing with
  this type of execution isolation strategy. This is mainly used when leveraging the `TenacityObservableCommand`.
* [Breakerbox](https://github.com/yammer/breakerbox) will have a corresponding update to this release to enable configuration it as well.

0.5.2
--------------
* [1.4.3 Hystrix](https://github.com/Netflix/Hystrix/blob/master/CHANGELOG.md#version-143-maven-central-bintray)

0.5.1
--------------
* [1.4.1 Hystrix](https://github.com/Netflix/Hystrix/blob/master/CHANGELOG.md#version-141-maven-central-bintray)

0.5.0
--------------
* [1.4.0 Hystrix](https://github.com/Netflix/Hystrix/blob/master/CHANGELOG.md#version-140-maven-central-bintray)
* TenacityObservableCommand is now available. This is _NOT_ executed on a separate threadpool, like `TenacityCommand` does, but instead leverage the [semaphore-isolated](https://github.com/Netflix/Hystrix/wiki/Configuration#thread-or-semaphore) execution strategy. It does support timeouts and these are handled by
  a separate thread `HystrixTimer`. These timeouts will behave exactly like they did with the thread-isolated execution strategy or when using `TenacityCommand`.
  Here you can read more about [Reactive Commands](https://github.com/Netflix/Hystrix/wiki/How-To-Use#reactive-commands)

0.4.5
--------------
* Added `TenacityJerseyClient` and `TenacityJerseyClientBuilder` to reduce configuration complexity when using Tenacity
  and `JerseyClient`. At the moment these two have competing timeout configurations that can end up looking like application exceptions
  when they are simply `TimeoutException`s being thrown by JerseyClient. `TenacityJerseyClient` aims to fix this by adjusting the socket read timeout
  on a per-request basis on the currently set execution timeout value for resources built from `TenacityJerseyClient` and its associated
  `TenacityPropertyKey`

0.4.4
--------------
* Hystrix 1.3.20

0.4.3
--------------
* Hystrix 1.3.19

0.4.2
--------------
* Removed registration of `MetricsPublisher` in the `TenacityTestRule` as it was breaking application test rule tests and wasn't necessary.

0.4.1
--------------
* `TenacityExceptionMapper` and `TenacityContainerExceptionMapper` now use a shared check to ensure that HystrixRuntimeExceptions are handled
  the same.
* Added a test to explicitly ensure that Hystrix Timeouts are handled appropriately by the ExceptionMapper
* Added a workaround for `HystrixPlugin.UnitTest.reset()` not reseting the static state correctly.

0.4.0
-----
* Changed `TenacityBundle` to be a `TenacityConfiguredBundle` and streamlined the tenacity-application integration process. This means:
  when declaring `TenacityPropertyKey` instances, there is access to the configuration class
  manual registering of configurations is no longer necessary.

0.3.6
-----
* Hystrix 1.3.18

0.3.5
-------------
* Adding 95/98 to the latencies. 
* Fixed bug where we are no longer publishing HystrixThreadPool metrics.

0.3.4
-------------
* Adding 99.9 to the latencies. Hystrix by default maxes out at 99.5 which is not consistent with Coda Hale metrics

0.3.3
--------------
* Dropwizard 0.7.1
* Force hystrix-codahale to depend on metrics 3.0.2, until [pull request 279](https://github.com/Netflix/Hystrix/pull/279) is merged
* Upgrade to findbugs 2.5.4
* Merged pull request 8. This adds a bunch of tests to test failure behavioral differences between execute()/queue()/observe()

0.3.2
-----
* Under high contention it's possible for HystrixThreadPoolMetrics to be associated with an incorrect TheadPoolExecutor.
This manifests itself as showing the incorrect metrics because the executor being used by Hystrix is different from the one
being used to supply metrics. As a temporary fix we now ensure that for any given ThreadPoolKey we only ever construct one pool.
This will be removed once it's fixed in upstream Hystrix. [pull request 270](https://github.com/Netflix/Hystrix/pull/270)

0.3.1
-----
* tenacity-client incorrectly captured metrics
* Hystrix 1.3.16
* maven-enforcer-plugin

0.3.0
--------------
* Supporting dropwizard 0.7.0
* 0.2.x now will only have fixes for the deprecated dropwizard <0.7.0



Dropwizard 0.6.x Releases
=========================
0.2.8
-----
* Hystrix 1.3.18

0.2.7
-------------
* Adding 95/98 to the latencies. 
* Fixed bug where we are no longer publishing HystrixThreadPool metrics.

0.2.6
-------------
* Adding 99.9 to the latencies. Hystrix by default maxes out at 99.5 which is not consistent with Coda Hale metrics

0.2.5
-----
* Under high contention it's possible for HystrixThreadPoolMetrics to be associated with an incorrect TheadPoolExecutor.
This manifests itself as showing the incorrect metrics because the executor being used by Hystrix is different from the one
being used to supply metrics. As a temporary fix we now ensure that for any given ThreadPoolKey we only ever construct one pool.
This will be removed once it's fixed in upstream Hystrix. [pull request 270](https://github.com/Netflix/Hystrix/pull/270)

0.2.4
-----
* Hystrix 1.3.15
* Generics lacking from some classes.

0.2.3
-----
* Created ExceptionLoggingCommandHook which passes thrown exceptions to the appropriate, registered ExceptionLogger
* Added HystrixCommandExecutionHook to TenacityBundleBuilder
* Created DefaultExceptionLogger, which just logs everything
* Created tenacity-jdbi module to house DBIExceptionLogger and SQLExceptionLogger

0.2.2
------
* Upgrade Hystrix to 1.3.13

0.2.1
--------------
* Upgrade Hystrix to 1.3.9


0.2.0
-----
* Initial release
