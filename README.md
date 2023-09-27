# React Component Standards
A set of patterns & standards to build scalable components across large teams.

## Why
We've had for years standards like airbnb amazing style guides/standards as well as packages like prettier. Though I noticed through my own interactions building and growing teams with large sets of components I needed more. Some of this is preference after years of building front end applications but I try to keep it grounded in solid reasoning. Hopefully this will help other teams as they are scaling there front end teams.

## Goals
- Build components faster
- Reduce code drift
- Levels up junior/mid-level engineers
- Faster onboarding
- Focus on hard logic problems and not structure


## Implementation

- [] Conceptual Draft
- [] Component Examples
- [] Strategy & Reasoning

### Concepts

- Naming
- Structure
- Code Patterns

### Component Structure

```
BaseComponent
- BaseComponent.view.tsx 
- BaseComponent.data.tsx
- BaseComponent.module.css
- index.tsx
-- MyNestedComponent
  - MyNestedComponent.view.tsx 
  - MyNestedComponent.data.tsx
  - MyNestedComponent.module.css
  - index.tsx
```

### Decision Guidelines
#### Explicit is better than Implicit
When naming things being a bit more explicit in the description of the item is usually better than generalized names. This reduces the cognative load when understanding what's going on in a peice of code or looking through logs. 
> You're not writing this for how'll you'll understand it now, but 6 months from now when you've totally forgot what the heck is going on. -someone famous

Examples:
```
Bad:
<Primary />;

Good:
<PrimaryLayout />
```

**Exceptions:**
As is the case there are always exceptions to rules. In this case when the point is to have generalized components for buttons, lists, tables, etc... It's more than fine to do so.



## Feedback
Please submit any feedback you may have! Would love to know if it helps.

