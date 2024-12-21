# Typescript

TypeScript (ts) is a superset of JavaScript (js) that adds type annotations.

The advantages of ts above js is the possibility to do strongly types code making it more readable and maintainable. An addition typescript increases development speed through improved IDE support, such as IntelliSense, providing features like autocomplete and real-time type checking.

# Usage
ts can be used together with node by installing the "typescript" package.
Having this you can run "tsc" to "compile" the ts into js, of a specific flavor, that can be executed in the browser.

## Configuration (tsconfig.json)
The behavior of the typescript compiler can be specified in a [tsconfig.json](https://www.typescriptlang.org/tsconfig/) file. A config file could look like this

```json
{
    "compilerOptions": {
        "module": "nodenext", // module system of project
        "target": "ES6", // Project will be compiled to this flavour of js
        "moduleResolution": "nodenext",
    }
}

```

### Module
nodenext support both ECMAScript import and CommonJS ```aquire```. But you have to conform to node import i.e. you have to include a file extension and can't do module imports.

