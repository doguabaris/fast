---
id: fast-foundation.singleton_2
title: singleton() function
hide_title: true
---
<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[@microsoft/fast-foundation](./fast-foundation.md) &gt; [singleton](./fast-foundation.singleton_2.md)

## singleton() function

Registers the `target` class as a singleton dependency; the class will only be created once. Each consecutive time the dependency is resolved, the same instance will be returned.

<b>Signature:</b>

```typescript
export declare function singleton<T extends Constructable>(target: T & Partial<RegisterSelf<T>>): T & RegisterSelf<T>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  target | T &amp; Partial&lt;[RegisterSelf](./fast-foundation.registerself.md)<!-- -->&lt;T&gt;&gt; | The class / constructor function to register as a singleton. |

<b>Returns:</b>

T &amp; [RegisterSelf](./fast-foundation.registerself.md)<!-- -->&lt;T&gt;

## Example


```ts
@singleton()
class Foo { }

```