---
title: TypeScript Reference for JS developers
---

# TypeScript Reference for JS developers<br/><br/>Glossary of keywords, operators, statements and directives<br/>

- [TypeScript Reference for JS developers<br/><br/>Glossary of keywords, operators, statements and directives<br/>](#typescript-reference-for-js-developersglossary-of-keywords-operators-statements-and-directives)
  - [Statements](#statements)
  - [Built-in Type Primitives](#built-in-type-primitives)
  - [Complex Types](#complex-types)
  - [Type and Interface Properties](#type-and-interface-properties)
  - [Functions](#functions)
    - [Arguments](#arguments)
    - [Type Guards and Assertion Functions](#type-guards-and-assertion-functions)
    - [Overloads](#overloads)
  - [Type Manipulation](#type-manipulation)
    - [Basic](#basic)
    - [Extension](#extension)
    - [Mapped Types](#mapped-types)
  - [Generics](#generics)
    - [Constrains](#constrains)
  - [Classes](#classes)
    - [Properties](#properties)
    - [Properties from JS](#properties-from-js)
    - [Constructor Parameter Properties](#constructor-parameter-properties)
    - [Extension](#extension-1)
    - [Decorators](#decorators)
  - [Utility Types](#utility-types)
  - [Comment Directives](#comment-directives)
    - [Enabling and Disabling Typescript](#enabling-and-disabling-typescript)
    - [References](#references)


Statements
----------

[`declare`](https://www.typescriptlang.org/docs/handbook/declaration-files/by-example.html), 
[`namespace`](https://www.typescriptlang.org/docs/handbook/namespaces.html)


Built-in Type Primitives
------------------------

[`boolean`](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html), 
[`string`](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html),
[`number`](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html),
[`undefined`](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html),
[`null`](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html),
[`any`](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html),
[`unknown`](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html),
[`never`](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html),
[`void`](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html),
[`bigint`](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html),
[`symbol`](https://www.typescriptlang.org/docs/handbook/symbols.html),
[`unique symbol`](https://www.typescriptlang.org/docs/handbook/symbols.html#unique-symbol)


Complex Types
-------------

[`|`](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html#union-types),
[`Array[]`](https://www.typescriptlang.org/docs/handbook/basic-types.html#array),
[`Tuple[]`](https://www.typescriptlang.org/docs/handbook/2/objects.html#tuple-types),
[`type`](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html#type-aliases),
[`interface`](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html#interfaces),
[`enum`](https://www.typescriptlang.org/docs/handbook/enums.html)


Type and Interface Properties
-----------------

[`property?: Type`](https://www.typescriptlang.org/docs/handbook/2/objects.html#optional-properties)

[`readonly property: Type`](https://www.typescriptlang.org/docs/handbook/2/objects.html#readonly-properties)

[`(...args): Type`](https://www.typescriptlang.org/docs/handbook/2/functions.html#call-signatures)

[`new(s: Type)`](https://www.typescriptlang.org/docs/handbook/2/functions.html#construct-signatures)

[`[key: Type]: Type;`](https://www.typescriptlang.org/docs/handbook/2/objects.html#index-signatures)


Functions
---------

### Arguments

[`{ (this: Type): Type }`](https://www.typescriptlang.org/docs/handbook/2/functions.html#declaring-this-in-a-function)

[`{ (...args: Type[]): Type }`](https://www.typescriptlang.org/docs/handbook/2/functions.html#rest-parameters-and-arguments)

### Type Guards and Assertion Functions

[`is`](https://www.typescriptlang.org/docs/handbook/2/narrowing.html#using-type-predicates),
[`asserts condition`](https://www.typescriptlang.org/docs/handbook/release-notes/typescript-3-7.html#assertion-functions),
[`asserts value is Type`](https://www.typescriptlang.org/docs/handbook/release-notes/typescript-3-7.html#assertion-functions)

### Overloads

[overloads](https://www.typescriptlang.org/docs/handbook/2/functions.html#function-overloads)


Type Manipulation
-----------------

### Basic
[`!`](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html#non-null-assertion-operator-postfix-)

[`as`](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html#type-assertions)

[`as const`](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html#literal-inference)

[`Type[key]`](https://www.typescriptlang.org/docs/handbook/2/indexed-access-types.html)

[`typeof`](https://www.typescriptlang.org/docs/handbook/2/typeof-types.html)

[`keyof`](https://www.typescriptlang.org/docs/handbook/2/keyof-types.html),

[`extends Type ? IfTrue : IfFalse`](https://www.typescriptlang.org/docs/handbook/2/conditional-types.html#inferring-within-conditional-types)

[`infer`](https://www.typescriptlang.org/docs/handbook/release-notes/typescript-2-8.html#type-inference-in-conditional-types)

### Extension

[`&`](https://www.typescriptlang.org/docs/handbook/2/objects.html#intersection-types),
[`extends`](https://www.typescriptlang.org/docs/handbook/2/objects.html#extending-types),
[merging](https://www.typescriptlang.org/docs/handbook/declaration-merging.html#merging-interfaces)

### Mapped Types

[`[Property in keyof Type]: Type;`](https://www.typescriptlang.org/docs/handbook/2/mapped-types.html)

[`-readonly [Property in keyof Type]: Type[Property];`](https://www.typescriptlang.org/docs/handbook/2/mapped-types.html#mapping-modifiers)

[`readonly [Property in keyof Type]: Type[Property];`](https://www.typescriptlang.org/docs/handbook/2/mapped-types.html#mapping-modifiers)

[`[Property in keyof Type]-?: Type[Property];`](https://www.typescriptlang.org/docs/handbook/2/mapped-types.html#mapping-modifiers)

[`[Property in keyof Type]?: Type[Property];`](https://www.typescriptlang.org/docs/handbook/2/mapped-types.html#mapping-modifiers)

[`[Properties in keyof Type as NewKeyType]: Type[Properties]`](https://www.typescriptlang.org/docs/handbook/2/mapped-types.html#key-remapping-via-as)


Generics
--------

[`interface NewType<Type>`](https://www.typescriptlang.org/docs/handbook/2/objects.html#generic-object-types)

[`type NewType<Type>`](https://www.typescriptlang.org/docs/handbook/2/objects.html#generic-object-types)

[`{ <Type>(arg: Type): Type }`](https://www.typescriptlang.org/docs/handbook/2/generics.html#generic-types)

[`class Class<Type>`](https://www.typescriptlang.org/docs/handbook/2/generics.html#generic-classes)

### Constrains

[`<Type extends OtherType>`](https://www.typescriptlang.org/docs/handbook/2/generics.html#generic-constraints)

Classes
-------

### Properties

[`property?: Type`](https://www.typescriptlang.org/docs/handbook/2/classes.html#this-based-type-guards)

[`property!: Type`](https://www.typescriptlang.org/docs/handbook/2/classes.html#fields)

[`readonly property: Type`](https://www.typescriptlang.org/docs/handbook/2/classes.html#readonly)

[`[key: Type]: Type`](https://www.typescriptlang.org/docs/handbook/2/classes.html#index-signatures)

[`private property: Type`](https://www.typescriptlang.org/docs/handbook/2/classes.html#private)

[`protected property: Type`](https://www.typescriptlang.org/docs/handbook/2/classes.html#protected)

[`declare property: Type`](https://www.typescriptlang.org/docs/handbook/2/classes.html#type-only-field-declarations)

### Properties from JS

[`#property: Type`](https://www.typescriptlang.org/docs/handbook/2/classes.html#caveats)

[`get property(): Type`](https://www.typescriptlang.org/docs/handbook/2/classes.html#getters--setters)

[`set property(...args): Type`](https://www.typescriptlang.org/docs/handbook/2/classes.html#getters--setters)

[`static property: Type`](https://www.typescriptlang.org/docs/handbook/2/classes.html#static-members)

[`static {...}`](https://www.typescriptlang.org/docs/handbook/2/classes.html#static-blocks-in-classes)

### Constructor Parameter Properties

[`constructor(parameter arg: Type)`](https://www.typescriptlang.org/docs/handbook/2/classes.html#parameter-properties)

### Extension

[`implements`](https://www.typescriptlang.org/docs/handbook/2/classes.html#class-heritage)

[`extends`](https://www.typescriptlang.org/docs/handbook/2/classes.html#extends-clauses)

[`abstract`](https://www.typescriptlang.org/docs/handbook/2/classes.html#abstract-classes-and-members)

### Decorators

[`@decorator class Class`](https://www.typescriptlang.org/docs/handbook/decorators.html#class-decorators)

[`@decorator property(...args) {...}`](https://www.typescriptlang.org/docs/handbook/decorators.html#class-decorators)

[`@decorator() property`](https://www.typescriptlang.org/docs/handbook/decorators.html#property-decorators)

[`property(@decorator arg: Type) {...}`](https://www.typescriptlang.org/docs/handbook/decorators.html#parameter-decorators)


Utility Types
-------------

[`Partial<Type>`](https://www.typescriptlang.org/docs/handbook/utility-types.html#partialtype)

[`Required<Type>`](https://www.typescriptlang.org/docs/handbook/utility-types.html#requiredtype)

[`Readonly<Type>`](https://www.typescriptlang.org/docs/handbook/utility-types.html#readonlytype)

[`Record<Keys, Type>`](https://www.typescriptlang.org/docs/handbook/utility-types.html#recordkeys-type)

[`Pick<Type, Keys>`](https://www.typescriptlang.org/docs/handbook/utility-types.html#picktype-keys)

[`Omit<Type, Keys>`](https://www.typescriptlang.org/docs/handbook/utility-types.html#omittype-keys)

[`Exclude<UnionType, ExcludedMembers>`](https://www.typescriptlang.org/docs/handbook/utility-types.html#excludeuniontype-excludedmembers)

[`Extract<Type, Union>`](https://www.typescriptlang.org/docs/handbook/utility-types.html#extracttype-union)

[`NonNullable<Type>`](https://www.typescriptlang.org/docs/handbook/utility-types.html#nonnullabletype)

[`Parameters<Type>`](https://www.typescriptlang.org/docs/handbook/utility-types.html#parameterstype)

[`ConstructorParameters<Type>`](https://www.typescriptlang.org/docs/handbook/utility-types.html#constructorparameterstype)

[`ReturnType<Type>`](https://www.typescriptlang.org/docs/handbook/utility-types.html#returntypetype)

[`InstanceType<Type>`](https://www.typescriptlang.org/docs/handbook/utility-types.html#instancetypetype)

[`ThisParameterType<Type>`](https://www.typescriptlang.org/docs/handbook/utility-types.html#thisparametertypetype)

[`OmitThisParameter<Type>`](https://www.typescriptlang.org/docs/handbook/utility-types.html#omitthisparametertype)

[`ThisType<Type>`](https://www.typescriptlang.org/docs/handbook/utility-types.html#thistypetype)

[`Uppercase<StringType>`](https://www.typescriptlang.org/docs/handbook/2/template-literal-types.html#uppercasestringtype)

[`Lowercase<StringType>`](https://www.typescriptlang.org/docs/handbook/2/template-literal-types.html#lowercasestringtype)

[`Capitalize<StringType>`](https://www.typescriptlang.org/docs/handbook/2/template-literal-types.html#capitalizestringtype)

[`Uncapitalize<StringType>`](https://www.typescriptlang.org/docs/handbook/2/template-literal-types.html#uncapitalizestringtype)


Comment Directives
------------------

### Enabling and Disabling Typescript

[`// @ts-ignore`](https://www.typescriptlang.org/docs/handbook/release-notes/typescript-2-6.html#suppress-errors-in-ts-files-using--ts-ignore-comments)

[`// @ts-check`](https://www.typescriptlang.org/docs/handbook/intro-to-js-ts.html#ts-check.html#suppress-errors-in-ts-files-using--ts-ignore-comments)

[`// @ts-nocheck`](https://www.typescriptlang.org/docs/handbook/release-notes/typescript-3-7.html#-ts-nocheck-in-typescript-files)

[`// @ts-expect-error`](https://www.typescriptlang.org/docs/handbook/release-notes/typescript-3-9.html#-ts-expect-error-comments)

### References

[`/// <reference path="..." />`](https://www.typescriptlang.org/docs/handbook/triple-slash-directives.html#-reference-path-)

[`/// <reference types="..." />`](https://www.typescriptlang.org/docs/handbook/triple-slash-directives.html#-reference-types-)

[`/// <reference lib="..." />`](https://www.typescriptlang.org/docs/handbook/triple-slash-directives.html#-reference-lib-)

[`/// <reference no-default-lib="true"/>`](https://www.typescriptlang.org/docs/handbook/triple-slash-directives.html#-reference-no-default-libtrue)

[`/// <amd-module />`](https://www.typescriptlang.org/docs/handbook/triple-slash-directives.html#-amd-module-)

[`/// <amd-dependency />`](https://www.typescriptlang.org/docs/handbook/triple-slash-directives.html#-amd-dependency-)
