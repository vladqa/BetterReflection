# Compatibility with native reflection API

The progress of compatibility can also be tracked in issue [#7](https://github.com/Roave/BetterReflection/issues/7).

## ReflectionClass

| Method | Supported |
|--------|-----------|
| getConstant | :heavy_check_mark: Yes (the `::class` constant is now resolved correctly) |
| getConstants | :heavy_check_mark: Yes |
| getConstructor | :heavy_check_mark: Yes |
| getDefaultProperties | :heavy_check_mark: Yes |
| getDocComment | :heavy_check_mark: Yes |
| getEndLine | :heavy_check_mark: Yes |
| getExtension | :x: No - extensions are not supported ([#15](https://github.com/Roave/BetterReflection/issues/15)) |
| getFileName | :heavy_check_mark: Yes |
| getInterfaceNames | :heavy_check_mark: Yes  |
| getInterfaces | :heavy_check_mark: Yes  |
| getMethod | :heavy_check_mark: Yes |
| getMethods | :heavy_check_mark: Yes |
| getModifiers | :heavy_check_mark: Yes |
| getName | :heavy_check_mark: Yes |
| getNamespaceName | :heavy_check_mark: Yes |
| getParentClass | :heavy_check_mark: Yes |
| getProperties | :heavy_check_mark: Yes |
| getProperty | :heavy_check_mark: Yes |
| getShortName | :heavy_check_mark: Yes |
| getStartLine | :heavy_check_mark: Yes |
| getStaticProperties | :x: No - would require loading ([#14](https://github.com/Roave/BetterReflection/issues/14)) |
| getStaticPropertyValue | :x: No - would require loading ([#14](https://github.com/Roave/BetterReflection/issues/14)) |
| getTraitAliases | :heavy_check_mark: Yes |
| getTraitNames | :heavy_check_mark: Yes |
| getTraits | :heavy_check_mark: Yes |
| hasConstant | :heavy_check_mark: Yes |
| hasMethod | :heavy_check_mark: Yes |
| hasProperty | :heavy_check_mark: Yes |
| implementsInterface | :heavy_check_mark: Yes |
| inNamespace | :heavy_check_mark: Yes |
| isAbstract | :heavy_check_mark: Yes |
| isCloneable | :heavy_check_mark: Yes |
| isFinal | :heavy_check_mark: Yes |
| isInstance | :heavy_check_mark: Yes  |
| isInstantiable | :heavy_check_mark: Yes  |
| isInterface | :heavy_check_mark: Yes |
| isInternal | :heavy_check_mark: Yes |
| isIterateable | :heavy_check_mark: Yes  |
| isSubclassOf | :heavy_check_mark: Yes  |
| isTrait | :heavy_check_mark: Yes |
| isUserDefined | :heavy_check_mark: Yes |
| newInstance | :x: No - would require loading ([#14](https://github.com/Roave/BetterReflection/issues/14)) |
| newInstanceArgs | :x: No - would require loading ([#14](https://github.com/Roave/BetterReflection/issues/14)) |
| newInstanceWithoutConstructor | :x: No - would require loading ([#14](https://github.com/Roave/BetterReflection/issues/14)) |
| setStaticPropertyValue | :x: No - would require loading ([#14](https://github.com/Roave/BetterReflection/issues/14)) |

## ReflectionFunctionAbstract

| Method | Supported |
|--------|-----------|
| getClosureScopeClass | :x: No - would require loading of the method itself ([#14](https://github.com/Roave/BetterReflection/issues/14)) |
| getClosureThis | :x: No - would require loading of the method itself ([#14](https://github.com/Roave/BetterReflection/issues/14)) |
| getDocComment | :heavy_check_mark: Yes |
| getEndLine | :heavy_check_mark: Yes |
| getExtension | :x: No - extensions are not supported ([#15](https://github.com/Roave/BetterReflection/issues/15)) |
| getExtensionName | :x: No - extensions are not supported ([#15](https://github.com/Roave/BetterReflection/issues/15)) |
| getFileName | :heavy_check_mark: Yes |
| getName | :heavy_check_mark: Yes |
| getNamespaceName | :heavy_check_mark: Yes |
| getNumberOfParameters | :heavy_check_mark: Yes |
| getNumberOfRequiredParameters | :heavy_check_mark: Yes |
| getParameters | :heavy_check_mark: Yes |
| getShortName | :heavy_check_mark: Yes |
| getStartLine | :heavy_check_mark: Yes |
| getStaticVariables | :x: No - would require loading ([#14](https://github.com/Roave/BetterReflection/issues/14)) |
| inNamespace | :heavy_check_mark: Yes |
| isClosure | :heavy_check_mark: Yes |
| isDeprecated | :heavy_check_mark: Yes - but see issue ([#38](https://github.com/Roave/BetterReflection/issues/38)) |
| isGenerator | :heavy_check_mark: Yes |
| isInternal | :heavy_check_mark: Yes - but see issue ([#38](https://github.com/Roave/BetterReflection/issues/38)) |
| isUserDefined | :heavy_check_mark: Yes |
| isVariadic | :heavy_check_mark: Yes |
| returnsReference | :heavy_check_mark: Yes |
| getReturnType | :heavy_check_mark: Yes |
| hasReturnType | :heavy_check_mark: Yes |

## ReflectionMethod

| Method | Supported |
|--------|-----------|
| getClosure | :x: No - would require loading of the method itself ([#14](https://github.com/Roave/BetterReflection/issues/14)) |
| getDeclaringClass | :heavy_check_mark: Yes |
| getModifiers | :heavy_check_mark: Yes |
| getPrototype | :heavy_check_mark: Yes |
| invoke | :x: No - would require loading of the method itself ([#14](https://github.com/Roave/BetterReflection/issues/14)) |
| invokeArgs | :x: No - would require loading of the method itself ([#14](https://github.com/Roave/BetterReflection/issues/14)) |
| isAbstract | :heavy_check_mark: Yes |
| isConstructor | :heavy_check_mark: Yes |
| isDestructor | :heavy_check_mark: Yes |
| isFinal | :heavy_check_mark: Yes |
| isPrivate | :heavy_check_mark: Yes |
| isProtected | :heavy_check_mark: Yes |
| isPublic | :heavy_check_mark: Yes |
| isStatic | :heavy_check_mark: Yes |
| setAccessible | :x: No - would require loading of the method itself ([#14](https://github.com/Roave/BetterReflection/issues/14)) |
| _inherited methods_ | see `ReflectionFunctionAbstract` |

## ReflectionParameter

| Method | Supported |
|--------|-----------|
| allowsNull | :heavy_check_mark: Yes |
| canBePassedByValue | :heavy_check_mark: Yes |
| getClass | :heavy_check_mark: Yes |
| getDeclaringClass | :heavy_check_mark: Yes |
| getDeclaringFunction | :heavy_check_mark: Yes |
| getDefaultValue | :heavy_check_mark: Yes (*some assumptions are made) |
| getDefaultValueConstantName | :heavy_check_mark: Yes |
| getName | :heavy_check_mark: Yes |
| getPosition | :heavy_check_mark: Yes |
| isArray | :heavy_check_mark: Yes |
| isCallable | :heavy_check_mark: Yes |
| isDefaultValueAvailable | :heavy_check_mark: Yes |
| isDefaultValueConstant | :heavy_check_mark: Yes |
| isOptional | :heavy_check_mark: Yes |
| isPassedByReference | :heavy_check_mark: Yes |
| isVariadic | :heavy_check_mark: Yes |
| getType | :heavy_check_mark: Yes |
| hasType | :heavy_check_mark: Yes |

## ReflectionFunction

| Method | Supported |
|--------|-----------|
| getClosure | :x: No - would require actual compilation of the AST ([#14](https://github.com/Roave/BetterReflection/issues/14)) |
| invoke | :x: No - would require loading of the function itself ([#14](https://github.com/Roave/BetterReflection/issues/14)) |
| invokeArgs | :x: No - would require loading of the function itself ([#14](https://github.com/Roave/BetterReflection/issues/14)) |
| isDisabled | :heavy_check_mark: Yes - but see issue ([#38](https://github.com/Roave/BetterReflection/issues/38)) |
| _inherited methods_ | see `ReflectionFunctionAbstract` |

## ReflectionProperty

| Method | Supported |
|--------|-----------|
| getDeclaringClass | :heavy_check_mark: Yes |
| getDocComment | :heavy_check_mark: Yes |
| getModifiers | :heavy_check_mark: Yes |
| getName | :heavy_check_mark: Yes |
| getValue | :x: No - would require an instance of an object ([#14](https://github.com/Roave/BetterReflection/issues/14)) |
| isDefault | :heavy_check_mark: Yes |
| isPrivate | :heavy_check_mark: Yes |
| isProtected | :heavy_check_mark: Yes |
| isPublic | :heavy_check_mark: Yes |
| isStatic | :heavy_check_mark: Yes |
| setAccessible | :x: No - would require an instance of an object ([#14](https://github.com/Roave/BetterReflection/issues/14)) |
| setValue | :x: No - would require an instance of an object ([#14](https://github.com/Roave/BetterReflection/issues/14)) |

## ReflectionExtension

:x: Will not be implemented

## ReflectionZendExtension

:x: Will not be implemented

## ReflectionObject

:x: Will not be implemented

## ReflectionType

| Method | Supported |
|--------|-----------|
| __toString | :heavy_check_mark: Yes |
| allowsNull | :heavy_check_mark: Yes |
| isBuiltin | :heavy_check_mark: Yes |
