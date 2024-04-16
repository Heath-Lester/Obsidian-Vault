Recursion is a type of loop which occurs when a function references itself.

```javascript
function inception(number, end) {
	number++;
	if (number === end) {
		return number;
	} else {
		return inception(number, end);
	}
}
```


One of the dangers of using recursion is that the calling of the function over and over can cause the call stack, which tracks function calls, to become larger than it's maximum allocated space. This is known as a [[Stack Overflow]].

Recursive functions must have a way to break the recursion which will allow the call stack to pop the functions from it. This is called the `base case`.

```javascript
function inception(number, end) {
	number++;
	if (number === end) { // < Base Case
		return number;
	} else {
		return inception(number, end);
	}
}
```

Recursive functions also must contain the recursive case to allow the function to operate recursively.

```javascript
function inception(number, end) {
	number++;
	if (number === end) {
		return number;
	} else { // < Recursive Case
		return inception(number, end);
	}
}
```

In most cases a recursive function will have two returns.

There is a theory that all  recursive approaches can be implemented using an iterative approach. The drawback of recursion is the additional allocation of memory in the call stack with the benefit of readability or a smaller text footprint. Additionally, some languages implement [[Tail Call Optimization]] which allows recursive functions to be called without increasing the size of the call stack.

Recursion is generally a good approach for data structures with an unknown depth.

Every time you are using a tree or converting something into a tree, consider recursion.
1. Divided into a number of subproblems that are smaller instances of the same problem.
2. Each instance of the subproblem is identical in nature.
3. The solutions of each subproblem can be combined to solve the problem at hand.

Divide & Conquer using recursion.

## Tail Recursion

Tail recursion is the recursive call is returned with using only variables passed in through arguments instead of waiting for the result to complete an expression. 

This is a normal recursion where the recursive return is the result of a larger expression. The call stack is created by multiplying the input to the decrement. The call stack is popped as the results are multiplied to `x` in the recursive return.

```javascript
// Normal recursion
function recFactorial(x) {
	if (x <= 1) {
		return 1;
	} else {
		return x * recFactorial(x - 1);
		// Recursion call gets added to the call stack because
		// the expression requries its calculation
	}
}
```

```javascript
// Tail recursion
function tailFactorial(x, totalSoFar = 1) {
	if (x === 0) {
		return totalSoFar;
	} else {
		return tailFactorial(x - 1, totalSoFar * x);
		// Recursion call is not added to the call stack because
		// the calculations are provided as arguments into the next call.
	}
}
```

Because the tail recursion does not require the result of the next call, the function call in the call stack can be pruned or deallocated from memory.