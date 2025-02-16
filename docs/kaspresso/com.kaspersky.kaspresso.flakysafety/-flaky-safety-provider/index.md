[kaspresso](../../index.md) / [com.kaspersky.kaspresso.flakysafety](../index.md) / [FlakySafetyProvider](./index.md)

# FlakySafetyProvider

`interface FlakySafetyProvider`

The interface to provide the flaky safety functionality.

### Functions

| Name | Summary |
|---|---|
| [flakySafely](flaky-safely.md) | `abstract fun <T> flakySafely(action: () -> `[`T`](flaky-safely.md#T)`): `[`T`](flaky-safely.md#T)<br>`abstract fun <T> flakySafely(timeoutMs: `[`Long`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html)`? = null, intervalMs: `[`Long`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html)`? = null, allowedExceptions: `[`MutableSet`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-mutable-set/index.html)`<`[`Class`](https://developer.android.com/reference/java/lang/Class.html)`<out `[`Throwable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-throwable/index.html)`>>? = null, failureMessage: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`? = null, action: () -> `[`T`](flaky-safely.md#T)`): `[`T`](flaky-safely.md#T)<br>Invokes the given [action](flaky-safely.md#com.kaspersky.kaspresso.flakysafety.FlakySafetyProvider$flakySafely(kotlin.Function0((com.kaspersky.kaspresso.flakysafety.FlakySafetyProvider.flakySafely.T)))/action) flaky safely. |

### Inheritors

| Name | Summary |
|---|---|
| [BaseTestContext](../../com.kaspersky.kaspresso.testcases.core.testcontext/-base-test-context/index.md) | `open class BaseTestContext : `[`FlakySafetyProvider`](./index.md)`, `[`ComposeProvider`](../../com.kaspersky.kaspresso.compose/-compose-provider/index.md)`, `[`WebComposeProvider`](../../com.kaspersky.kaspresso.compose/-web-compose-provider/index.md)<br>Provides the Kaspresso functionality for "run" section: [Device](../../com.kaspersky.kaspresso.device/-device/index.md), [AdbServer](../../com.kaspersky.kaspresso.device.server/-adb-server/index.md), the [UiTestLogger](../../com.kaspersky.kaspresso.logger/-ui-test-logger.md) implementation for external developers. Also provides flaky safety, composing and web composing functionalities via implementing [FlakySafetyProvider](./index.md), [ComposeProvider](../../com.kaspersky.kaspresso.compose/-compose-provider/index.md) and [WebComposeProvider](../../com.kaspersky.kaspresso.compose/-web-compose-provider/index.md) interfaces. |
| [FlakySafeDataBehaviorInterceptor](../../com.kaspersky.kaspresso.interceptors.behavior.impl.flakysafety/-flaky-safe-data-behavior-interceptor/index.md) | `class FlakySafeDataBehaviorInterceptor : `[`DataBehaviorInterceptor`](../../com.kaspersky.kaspresso.interceptors.behavior/-data-behavior-interceptor.md)`, `[`FlakySafetyProvider`](./index.md)<br>The implementation of [DataBehaviorInterceptor](../../com.kaspersky.kaspresso.interceptors.behavior/-data-behavior-interceptor.md) and [FlakySafetyProvider](./index.md) interfaces. Provides system flaky safety functionality for [DataInteraction.check](#) calls. |
| [FlakySafetyProviderImpl](../-flaky-safety-provider-impl/index.md) | `class FlakySafetyProviderImpl : `[`FlakySafetyProvider`](./index.md)<br>The implementation of the [FlakySafetyProvider](./index.md) interface. |
| [FlakySafeViewBehaviorInterceptor](../../com.kaspersky.kaspresso.interceptors.behavior.impl.flakysafety/-flaky-safe-view-behavior-interceptor/index.md) | `class FlakySafeViewBehaviorInterceptor : `[`ViewBehaviorInterceptor`](../../com.kaspersky.kaspresso.interceptors.behavior/-view-behavior-interceptor.md)`, `[`FlakySafetyProvider`](./index.md)<br>The implementation of [ViewBehaviorInterceptor](../../com.kaspersky.kaspresso.interceptors.behavior/-view-behavior-interceptor.md) and [FlakySafetyProvider](./index.md) interfaces. Provides system flaky safety functionality for [ViewInteraction.perform](#) and [ViewInteraction.check](#) calls. |
| [FlakySafeWebBehaviorInterceptor](../../com.kaspersky.kaspresso.interceptors.behavior.impl.flakysafety/-flaky-safe-web-behavior-interceptor/index.md) | `class FlakySafeWebBehaviorInterceptor : `[`WebBehaviorInterceptor`](../../com.kaspersky.kaspresso.interceptors.behavior/-web-behavior-interceptor.md)`, `[`FlakySafetyProvider`](./index.md)<br>The implementation of [WebBehaviorInterceptor](../../com.kaspersky.kaspresso.interceptors.behavior/-web-behavior-interceptor.md) and [FlakySafetyProvider](./index.md) interfaces. Provides system flaky safety functionality for [Web.WebInteraction.perform](#) and [Web.WebInteraction.check](#) calls. |
