---
created:
  - 2024-03-09 11:21
tags:
  - react
  - programming
---
# useEffect()

`useEffect()` hook accepts 2 arguments:

```javascript 
useEffect(callback, [dependencies]);
```

- `callback` is a function that contains the side-effect logic. `callback` is executed right after the DOM update.
- `dependencies` is an optional array of dependencies. `useEffect()` executes `callback` only if the dependencies have changed between renderings.

![[useEffect.png]]

```javascript
// not provided dependency
function MyComponent(){
	useEffect(() => {
		// Runs after EVERY rendering
	});
}

// provided empty dependency
function MyComponent(){
	useEffect(() => {
		// Runs ONCE on the initial render
	}, []);
}

// dependencies provided
function MyComponent(prop){
	const [state, setState] = useState('');
	useEffect(() => {
		// Runs ONCE on the initial render
		// and will render if the prop or state changes
	}, [prop, state]);
}
```
