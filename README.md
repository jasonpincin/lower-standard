# JavaScript Lower Standard Style

This is a slightly less strict fork of
[standard](https://github.com/feross/standard)

## Install

```bash
npm install lower-standard
```

## Rules

More relaxed than regular standard. Code should be enjoyable to write and pretty
to look at. A lot of the big ticket items are the same as standard, for example:

- **Single quotes for strings** – except to avoid escaping
- **No unused variables** – this one catches *tons* of bugs!
- **No semicolons**
- **Never start a line with `(` or `[`**
  - This is the **only** gotcha with omitting semicolons – *automatically checked for you!*
  - [More details][4]
- **Space after keywords** `if (condition) { ... }`
- **Space after function name** `function name (arg) { ... }`
- Always use `===` instead of `==` – but `obj == null` is allowed to check `null || undefined`.
- Always handle the node.js `err` function parameter
- Always prefix browser globals with `window` – except `document` and `navigator` are okay
  - Prevents accidental use of poorly-named browser globals like `open`, `length`,
    `event`, and `name`.
- **And [more goodness][5]** – *give `standard` a try today!*

The biggest differences:

- **2 spaces** – for indentation
- **function names** - warn if missing - seriously, name your functions,
  the person debugging production will thank you
- **arrow parens if needed** `array.filter(x => x)` is nicer to look at
- **stroustrup brace style** down with 1tbs!
- **do not force curlys** `if (bool) doSomething()` is nice looking
- **proper generator start position** - `function *sayHello() {}`
- **line up key colons**
- **max line length 80** - keep stuff readable on small screens
- **allow case fallthroughs** - why disable this feature? Just use `if` if you
  don't like it
- **no opinion on onevar**
