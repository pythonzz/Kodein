[com.github.salomonbrys.kodein](../../../index.md) / [Kodein](../../index.md) / [Builder](../index.md) / [ConstantBinder](index.md) / [withGeneric](.)

# withGeneric

`inline infix fun <reified T : Any> withGeneric(value: T): Unit`

Binds the previously given tag to the given instance.

T generics will be kept.

### Parameters

`T` - The type of value to bind.

`value` - The instance to bind.