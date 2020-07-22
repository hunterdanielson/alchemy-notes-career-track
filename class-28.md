# Alchemy Reading Notes

## Class 28

Architectural Patterns are high-level strategies that concern large-scale components, the global properties and mechanisms of a system.
A single architecture can contain several Architectural Styles, and each Architectural Style can make use of several Architectural Patterns. An Architecture Patterns can be a subset of an Architectural Styles targeting a specific scope.

The container and presentation pattern splits code into two distinct places:

containers : are stateful components that contain your business login
presentations : are stateless components that present your data

When the Container/Presentation pattern first became popular all containers were class based components. At that time state and lifecycle methods were only available within class components. Since containers are responsible for managing state and fetching data (lifecycle methods) they were exclusively written as class components. This helped highlight the dichotomy between container components (classes) and presentational components (functions).

Use functional components if you are writing a presentational component which doesn’t have its own state or needs to access a lifecycle hook. Otherwise you can stick to class components or take a look into the library recompose which allows you to write functional components and enhance them with a state or lifecycle hooks with HOCs!