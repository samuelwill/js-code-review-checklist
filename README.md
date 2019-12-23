## Javascript Code Review Checklist

### General
- [ ] All new Javascript code is written in ES2015+
- [ ] `const` is used by default. `let` is used only if a variable must change. `var` is not used
- [ ] Comparisons are done using `===` instead of `==` to avoid type coercion
- [ ] Native higher-order functions like `map`, `reduce`, `filter`, etc are used over imperative loops
- [ ] `Object.keys`, `Object.values`, `Object.entries` are used to iterate over objects
- [ ] Spread operator `…` is used to copy arrays
- [ ] Layouts are achieved using `Flexbox` or `Grid`, not Javascript
- [ ] Any architecture / design concerns have been logged to a Developer Backlog

### Maintainence
- [ ] Functions, classes and modules are small, focused and follow the Single Responsibility Principle
- [ ] Modules, classes, functions and variables have clear, descriptive names
- [ ] Clear, descriptive variable, method and class names are used instead of comments
- [ ] Higher order function predicates have been extracted and given great names
- [ ] Functions only operate at one level of abstraction
- [ ] Complex conditionals have been extracted into well-named methods
- [ ] Functions avoid side-effects / functions `return` values instead of mutating values
- [ ] All Javascript has been linted and passes spec

### Performance and Scalability
- [ ] New scripts are loaded in HTML using `async` or `defer`
- [ ] DOM events have been throttled or debounced
- [ ] DOM size has been reduced as much as possible
- [ ] DOM references have been cached
- [ ] Scope chains / closures have been minimized as much as possible
- [ ] Lists have been virtualized
- [ ] New layouts are achieved using `Flexbox` or `Grid`
- [ ] New functionality has been profiled used the Chrome “Performance” tab to check for long running scripts and layout thrashing
- [ ] `async` / `await` is used over promises or callbacks
- [ ] Event delegation has been used to reduce the number of DOM event listeners
