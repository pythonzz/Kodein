[com.github.salomonbrys.kodein.erased](index.md) / [instance](.)

# instance

`inline fun <reified T : Any> `[`KodeinInjectedBase`](../com.github.salomonbrys.kodein/-kodein-injected-base/index.md)`.instance(tag: Any? = null): `[`InjectedProperty`](../com.github.salomonbrys.kodein/-injected-property/index.md)`<T>`

Gets a lazy instance for the given type and tag.

The returned property should not be accessed before calling [KodeinInjectedBase.inject](../com.github.salomonbrys.kodein/-kodein-injected-base/inject.md).

T generics will be erased!

### Parameters

`T` - The type of object to retrieve.

`tag` - The bound tag, if any.

### Exceptions

`KodeinInjector.UninjectedException` - When accessing the property, if it was accessed before calling [KodeinInjectedBase.inject](../com.github.salomonbrys.kodein/-kodein-injected-base/inject.md).

**Receiver**
Either a [KodeinInjector](../com.github.salomonbrys.kodein/-kodein-injector/index.md) instance or a [KodeinInjected](../com.github.salomonbrys.kodein/-kodein-injected.md) class.

**Return**
A lazy property that yields a `T`.

`inline fun <reified T : Any> `[`CurriedInjectorFactory`](../com.github.salomonbrys.kodein/-curried-injector-factory/index.md)`<*>.instance(tag: Any? = null): Lazy<T>`

Gets a lazy instance of `T` for the given tag from a factory with an `A` argument.

The returned property should not be accessed before calling [KodeinInjectedBase.inject](../com.github.salomonbrys.kodein/-kodein-injected-base/inject.md).

T generics will be erased!

### Parameters

`T` - The type of object to retrieve.

`tag` - The bound tag, if any.

### Exceptions

`KodeinInjector.UninjectedException` - When accessing the property, if it was accessed before calling [KodeinInjectedBase.inject](../com.github.salomonbrys.kodein/-kodein-injected-base/inject.md).

**Return**
A lazy property that yields a `T`.

`inline fun <reified T : Any> `[`Builder`](../com.github.salomonbrys.kodein/-kodein/-builder/index.md)`.instance(instance: T): `[`Provider`](../com.github.salomonbrys.kodein/-provider/index.md)`<T>`

Creates an instance provider: will always return the given instance.

T generics will be erased!

### Parameters

`T` - The type of the instance.

`instance` - The object that will always be returned.

**Return**
An instance provider ready to be bound.

`inline fun <reified T : Any> `[`LazyKodeinAwareBase`](../com.github.salomonbrys.kodein/-lazy-kodein-aware-base/index.md)`.instance(tag: Any? = null): Lazy<T>`

Gets a lazy instance for the given type and tag.

T generics will be erased!

### Parameters

`T` - The type of object to retrieve.

`tag` - The bound tag, if any.

### Exceptions

`Kodein.NotFoundException` - When accessing the property, if no provider was found.

`Kodein.DependencyLoopException` - When accessing the property, if the value construction triggered a dependency loop.

**Receiver**
Either a [LazyKodein](../com.github.salomonbrys.kodein/-lazy-kodein/index.md) instance or a [LazyKodeinAware](../com.github.salomonbrys.kodein/-lazy-kodein-aware.md) class.

**Return**
A lazy property that yields an instance of `T`.

`inline fun <reified T : Any> `[`CurriedLazyKodeinFactory`](../com.github.salomonbrys.kodein/-curried-lazy-kodein-factory/index.md)`<*>.instance(tag: Any? = null): Lazy<T>`

Gets a lazy instance of `T` for the given tag from a curried factory with an `A` argument.

T generics will be erased!

### Parameters

`T` - The type of object to retrieve.

`tag` - The bound tag, if any.

### Exceptions

`Kodein.NotFoundException` - When accessing the property, if no factory was found.

`Kodein.DependencyLoopException` - When accessing the property, if the value construction triggered a dependency loop.

**Return**
A lazy instance of `T`.

`inline fun <reified T : Any> `[`KodeinAwareBase`](../com.github.salomonbrys.kodein/-kodein-aware-base/index.md)`.instance(tag: Any? = null): T`

Gets an instance of `T` for the given type and tag.

Whether the returned object is a new instance at each call or not depends on the binding scope.

T generics will be erased!

### Parameters

`T` - The type of object to retrieve.

`tag` - The bound tag, if any.

### Exceptions

`Kodein.NotFoundException` - if no provider was found.

`Kodein.DependencyLoopException` - If the instance construction triggered a dependency loop.

**Receiver**
Either a [Kodein](../com.github.salomonbrys.kodein/-kodein/index.md) instance or a [KodeinAware](../com.github.salomonbrys.kodein/-kodein-aware.md) class.

**Return**
An instance.

`inline fun <reified T : Any> `[`CurriedKodeinFactory`](../com.github.salomonbrys.kodein/-curried-kodein-factory/index.md)`<*>.instance(tag: Any? = null): T`

Gets an instance of `T` for the given tag from a curried factory with an `A` argument.

Whether the returned object is a new instance at each call or not depends on the binding scope.

T generics will be erased!

### Parameters

`T` - The type of object to retrieve.

`tag` - The bound tag, if any.

### Exceptions

`Kodein.NotFoundException` - if no factory was found.

`Kodein.DependencyLoopException` - If the instance construction triggered a dependency loop.

**Return**
An instance.

