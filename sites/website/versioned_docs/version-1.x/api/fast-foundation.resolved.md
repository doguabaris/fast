---
id: fast-foundation.resolved
title: Resolved type
hide_title: true
---
<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[@microsoft/fast-foundation](./fast-foundation.md) &gt; [Resolved](./fast-foundation.resolved.md)

## Resolved type

Represents something resolved from a service locator.

<b>Signature:</b>

```typescript
export declare type Resolved<K> = K extends InterfaceSymbol<infer T> ? T : K extends Constructable ? InstanceType<K> : K extends ResolverLike<any, infer T1> ? T1 extends Constructable ? InstanceType<T1> : T1 : K;
```