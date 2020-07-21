# Alchemy Reading Notes

## Class 27

Reviewing setState in React was a nice refresher

Learning about Reconciliation was interesting. It's cool to learn about how developers thought about saving complexity from making something unusable for large computations in O(n^3) complexity down to O(n) complexity.

PropTypes was cool to learn about, although personally I don't see the point in using that over something like TypeScript if you are wanting to type things.

Testing refreshers were pretty neat.
Snapshot testing is always simpler to do than understand for me. 
Shallow testing makes it so that it does not have to rely on other components for the tests, and it calls componentDidMount/componentDidUpdate.
Render will render the HTML of a component you are testing, to allow for analysis on it.
Full DOM rendering is used when you have components that interact with DOM APIs or need to test components wrapped in higher order components.
