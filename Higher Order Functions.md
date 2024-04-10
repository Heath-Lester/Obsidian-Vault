https://en.wikipedia.org/wiki/Higher-order_function

A higher order function is a function used as an argument or a return value;

```ts
public foo(higherOrderFunction: () => any): () => any {
	higherOrderFunction();
	return () => {
		console.log("bar");
	}
}
```