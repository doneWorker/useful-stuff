# Imports

## Avoid Relative paths(i.e `../../../lib`)

use path aliases:

```json
// tsconfig.json or jsconfig.json
{
  "compilerOptions": {
    "baseUrl": ".",
    "paths": {
      "@/components/*": ["components/*"]
    }
  }
}
```

```js
// Before
import "../../components/Component";

// After
import "components/Component";
```

## Top-to-bottom rule:

- Frameworks / other third-party libraries
- Your js libraries
- css styles / svg icons / json / ...etc

# React components

- react component should be declared as arrow function
- react component should use object destructuring while receive the props
- while using typescript declare props right before declaring the component
- react component file should consist of less than 100 sloc (ideally 30-60)
- place unit tests in the same folder as component you testing. Name them "\*.test.[js|ts]"
- place _.css,_.scss files near the component

# Styled components

-

# Folder structure

-
