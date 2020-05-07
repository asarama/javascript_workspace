# How TypeScript Can Help

TypeScript is a superset of JavaScript.

The problem with JS:
 - JS was not designed to build big apps
 - JS was designed to make minor modifications to simple web pages
 - Support for many design patterns were excluded

 TypeScript tackles these problems by solving these problems and then compiling to JavaScript.

 The benefits of TS:
  - Static types
    - Aka variable types (not values) are immutable
  - Organizational support
    - Classes
    - Namespaces
    - Modules
    - Interfaces
  - Tooling support
    - Since TS is compiled we get better analysis of code

# Setting Up a TypeScript Development Environment

Make sure you have NodeJs installed.

Install the typescript complier `tsc`.

```bash
npm i -g typescript
```

# Writing TypeScript Applications

## Static Typing

TypeScript uses type inference when a type is not explicitly defined. The ```any``` type can be used when we do not want to set a single type for a variable.

```TypeScript
let some_string:string = "Hello";
let some_number:number = 12;

function some_function(some_string:string, some_number:number):string {
    return some_string + some_number.toString();
}
```

## Classes

```TypeScript
class Customer {
    name:string;
    isActive:boolean;

    constructor(name:string) {
        this.name = name;
        this.isActive = true;
    }

    private some_private_method() {

    }

    public some_public_method() {

    }

    protected some_protected_method() {

    }
}

class SpecialCustomer extends Customer {
    //...overload methods as required
}
```

## Modules

```TypeScript

// module.ts

export hello:number = 10;

// component.ts

import { hello } from './module.ts';

```