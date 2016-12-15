# TypeScript

###General info on TypeScript

**TS compiler**

The TypeScript compiler performs only file-local transformations on TypeScript programs and does not re-order variables declared in TypeScript. This leads to JavaScript output that closely matches the TypeScript input. TypeScript does not transform variable names, making tractable the direct debugging of emitted JavaScript. 

TypeScript optionally provides source maps, enabling source-level debugging. TypeScript tools typically emit JavaScript upon file save, preserving the test, edit, refresh cycle commonly used in JavaScript development.

```TypeScript
interface JQueryStatic {  
    get(url: string, callback: (data: string) => any);     
    (query: string): JQuery;  
}
```



The 'JQueryStatic' interface contains a bare function signature 
```typescript 
(query: string): JQuery;
```

The bare signature indicates that instances of the interface are callable. This example illustrates that TypeScript function types are just special cases of TypeScript object types. Specifically, function types are object types that contain one or more call signatures.
