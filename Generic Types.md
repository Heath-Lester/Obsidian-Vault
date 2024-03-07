Generic Types are language types non-specific. These can be used to make it so functions can use multiple types in their inputs and/or outputs. It can also be used in interfaces so that the extended classes or the specificed type can be non-specific

```ts
function identity(arg: any): any {  return arg;}
```

```ts
function createPair<S, T>(v1: S, v2: T): [S, T] {  
  return [v1, v2];  
}  
console.log(createPair<string, number>('hello', 42)); // ['hello', 42]
```

```java
/**
 * Generic version of the Box class.
 * @param <T> the type of the value being boxed
 */
public class Box<T> {
    // T stands for "Type"
    private T t;

    public void set(T t) { this.t = t; }
    public T get() { return t; }
}
```
