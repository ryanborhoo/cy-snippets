# VSCode Cypress Snippets

This cy-snippets is for Cypress code snippets.

## Installation

You can install this extension from VSCode marketplace, search for cy-snippets and install it.

## Requirements

Cypress code snippets support below files

- JavaScript (.js)
- TypeScript (.ts)

## Features

### Cypress Test Project Snippet: `!cyProject`

```javascript
describe("This is your test project title", () => {
  before(() => {
    // runs once before all tests
  });
  beforeEach(() => {
    // runs before every it() test block
  });
  afterEach(() => {
    // runs after every it() test block
  });
  after(() => {
    // runs once after all tests
  });
  context("This is your test suite title", () => {
    // -- Start: Cypress Tests --
    it("This is your test case one title", () => {
      // Write your test case one here
    });
    it("This is your test case two title", () => {
      // Write your test case two here
    });
  });
});
```

### Cypress Test Suite Snippet: `!cySuite`

```javascript
context("This is your test suite title", () => {
  before(() => {
    // runs once before all tests
  });
  beforeEach(() => {
    // runs before every it() test block
  });
  afterEach(() => {
    // runs after every it() test block
  });
  after(() => {
    // runs once after all tests
  });
  // -- Start: Cypress Tests --
  it("This is your test case one title", () => {
    // Write your test case one here
  });
  it("This is your test case two title", () => {
    // Write your test case two here
  });
});
```

### Cypress Test Case Snippet: `!cyTest`

```javascript
it("This is your test case title", () => {
  // Write your test case here
});
```

### Cypress API Call Snippet: `!cyAPI`

```javascript
cy.request({
  method: " ",
  url: " ",
  headers: { "Accept-Language": "en-us" },
});
```

### Cypress Command Snippet: `!cyComm`

```javascript
Cypress.Commands.add("Command name here", () => {
  // Write your command here
});
```

### Cypress Ignore Case Snippet: `!cyNoCase`

```javascript
{
  matchCase: false;
}
```

### Cypress Force Event Snippet: `!cyForce`

```javascript
{
  force: true;
}
```

### Cypress Check Element Visiable Snippet: `!cyVisiable`

```javascript
should("be.visible");
```

### Cypress Check Element Attribute Snippet: `!cyAttr`

```javascript
should("have.attr", "attributeName", "attributeVale");
```

### Cypress Assertions Expect: `!cyExpect`

```javascript
cy.get('selector').then(($element) => {
    expect($element).equal('expect result');
});
```
