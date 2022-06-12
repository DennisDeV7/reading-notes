# Introduction to React and Components

## Reading

### Component-Based Architecture

Most information in notes below is directly from the following website:
https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm

- "A component encapsulates functionality and behaviors of a software element into a reusable and self-deployable binary unit"
- Views of a component:
      - Object-oriented view
      - Conventional view
      - Process-related view
- Characteristics of Components
      - Reusability: Components are usually designed to be reused in different situations in different applications. However, some components may be designed for a specific task.
      - Replaceable: Components may be freely substituted with other similar components.
      - Not context specific: Components are designed to operate in different environments and contexts.
      - Extensible: A component can be extended from existing components to provide new behavior.
      - Encapsulated: A component depicts the interfaces, which allow the caller to use its functionality, and do not expose details of the internal processes or any internal variables or state.
      - Independent: Components are designed to have minimal dependencies on other components.
- Advantages:
      - Ease of deployment: as new compatible versions become available, it is easier to replace existing versions with no impact on the other components or the system as a whole.
      - Reduced cost: The use of third-party components allows you to spread the cost of development and maintenance.
      - Ease of development: Components implement well-known interfaces to provide defined functionality, allowing development without impacting other parts of the system.
      - Reusable: The use of reusable components means that they can be used to spread the development and maintenance cost across several applications or systems.
      - Modification of technical complexity: A component modifies the complexity through the use of a component container and its services.
      - Reliability: The overall system reliability increases since the reliability of each individual component enhances the reliability of the whole system via reuse.
      - System maintenance and evolution: Easy to change and update the implementation without affecting the rest of the system.
      - Independent: Independency and flexible connectivity of components. Independent development of components by different group in parallel. Productivity for the software development and future software development.

### Props and How to Use it in React

Site used for information:
https://itnext.io/what-is-props-and-how-to-use-it-in-react-da307f500da0

- "props is short for properties and is used for passing data from one component to another (parent to child)
- Props are used by following these three steps:
      1. Define an attribute and its value
      2. Pass the value to the child component
      3. Render the props data
- Props flow from parents to child

## Things I want to know more about