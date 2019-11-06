# Built-in Functions

Components come with a series of built-in functions that will make it easier to interact with them.

## Modify the HTML structure

```
static template ()
```

This function allows you to either get the HTML structure from a component, or set a new one to it.

### Examples

    monogatari.component ('main_screen').template (() => {
        return `
            <h1>My Awesome Game</h1>
            <main-menu></main-menu>
        `;
    });

## Running an arbitrary line of Monogatari

```
monogatari.run ("string")
```

Runs a line of the script as though it were a regular line in the script array. Can be invoked from the JavaScript development console for testing, such as `monogatari.run("jump myLabel")` if you want to rapidly test a particular label. This can also be used as part of a function if you need to do something specific or fancy. Up to you.
