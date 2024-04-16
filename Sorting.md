https://www.toptal.com/developers/sorting-algorithms

<iframe width="100%" src="https://www.youtube-nocookie.com/embed/kPRA0W1kECg?si=T1Kx7rFlykW5pvBb" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen style="border-radius: 4px; aspect-ratio: 16/9;"></iframe>


Sorting is not very important for small input data. Sorting is **very** important for large input data at the enterprise level. 

## Bubble Sort

Bubble sort does a side by side comparison that swaps places incrementally and executes again until the entire array has been looped through.

```typescript
const number = [99, 44, 6, 2, 1, 5, 63, 87, 283, 4, 0];

function bubbleSort(array: Array<number>): void {
	const length = array.length;
	for (let i = 0; i < length; i++) {
		for (let j = 0; j < length; j++) {
			if (array[j] > array[j+1]) {
				let temp = array[j];
				array[j] = array[j+1];
				array[j+1] = temp;
			}
		}
	}
}
```
