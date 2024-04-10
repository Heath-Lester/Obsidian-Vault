https://en.wikipedia.org/wiki/Closure_(computer_programming)

Closure is when a function is nested within the local scope of another function along with other variables.

The advantage of this is that a function within the scope can access variables in the outer function.

```ts
public foo(): number {
	let a: number = 10;
	return function () {
		a++;
		return a;
	}
}
```