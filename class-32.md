# Alchemy Reading Notes

## Class 32

### Custom Hooks

A custom Hook is a JavaScript function whose name starts with ”use” and that may call other Hooks

Hooks are JavaScript functions, but you need to follow two rules when using them.
- Only Call Hooks at the Top Level
  - Don’t call Hooks inside loops, conditions, or nested functions. Instead, always use Hooks at the top level of your React function. By following this rule, you ensure that Hooks are called in the same order each time a component renders. That’s what allows React to correctly preserve the state of Hooks between multiple useState and useEffect calls.
- Only Call Hooks from React Functions
  - Don’t call Hooks from regular JavaScript functions

[10 React Hooks Resource](https://blog.bitsrc.io/10-react-custom-hooks-you-should-have-in-your-toolbox-aa27d3f5564d)