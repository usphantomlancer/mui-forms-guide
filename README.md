# Material UI Forms

Material UI forms using json based schema
  
## Advantages and features
- Mui Components
- Built-in layouting
- Supports custom components
- Easily define field relationships and build advanced forms
- Load data from remote api

## Install

```bash
npm install mui-forms
```

## Basic Usage

### 1. Define your json schema
```typescript
const exampleSchema = {
    "fields": [{
        "name": "first_name",
        "meta": {
            "displayType": "text",
            "displayName": "First Name"
        }
    }, {
        "name": "last_name",
        "meta": {
            "displayType": "text",
            "displayName": "Last Name"
        }
    }]
}
```
### 2. Usage

```tsx
import React from 'react'

import MuiForms from 'mui-forms';

export function MyForm() {
    return (
        <MuiForms
            schema={exampleSchema}
            onSubmit={(formData) => {
              // submit data
            }}
        />
    );
}
```

### 3. Schema details
Check out the [file]([typescript-schema.md](https://github.com/manojadams/mui-forms/blob/master/typescript-schema.md))

## Contributions

Open source contribution is welcome.