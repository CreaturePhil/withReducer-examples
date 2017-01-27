# withReducer Examples

Application examples using `withReducer` function from
[recompose](https://github.com/acdlite/recompose) but reimplemented to use
with any framework.

The `withReducer` function creates a higher order component where
state updates are applied using a reducer function.

# Type

The type of `withReducer` is

```js
withReducer<S, A>(
  stateName: string,
  dispatchName: string,
  reducer: (state: S, action: A) => S,
  initialState: S
): HigherOrderComponent
```

```haskell
withReducer :: (State s, Action a, Component c) => String -> String -> ((s, a) -> a) -> s -> c
```

# Examples

- Counter: [React](creaturephil.github.io/withReducer-examples/counter/react-counter.html) | [Preact](creaturephil.github.io/withReducer-examples/counter/preact-counter.html) |
[Inferno](creaturephil.github.io/withReducer-examples/counter/inferno-counter.html)
- Todos: [React](creaturephil.github.io/withReducer-examples/todos/react-todos.html) | [Preact](creaturephil.github.io/withReducer-examples/todos/preact-todos.html) |
[Inferno](creaturephil.github.io/withReducer-examples/todos/inferno-todos.html)

# LICENSE

[MIT](LICENSE)
