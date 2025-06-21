# Show HN: Tree-hugger-JS — CSS Selectors for JavaScript AST Analysis and MCP

**Posted by chw9e on 2025-06-20**

I built a library that allows you to find code patterns using familiar CSS-like selectors and connected it to Claude via MCP so AI assistants can understand and refactor codebases.

## The Approach

### Find code patterns with intuitive selectors:

```js
const asyncFunctions = tree.findAll('function[async]');
const todoComments = tree.findAll('comment[text="TODO"]');
const reactHooks = tree.hooks(); // Built-in React support
```

### Chain smart transformations:

```js
tree.transform()
  .rename('oldFunction', 'newFunction')
  .removeUnusedImports()
  .toString();
```

## Key Features

- **CSS-like selectors:** `function[async]`, `class:has(method)`, `call[text*="fetch"]`
- **Semantic aliases:** Match functions with declarations, expressions, arrows, and methods
- **Smart transformations:** Rename identifiers, remove unused imports, insert code
- **Built-in queries:** Functions, classes, imports, React hooks, JSX components
- **TypeScript support:** Full parameter extraction with types
- **Scope analysis:** Track variable bindings and references

## MCP Integration

I built an MCP server that exposes these capabilities to AI assistants. For example, you can ask Claude:

> "Find all functions that use console.log and show me their parameters"

Claude can then:

1. Parse your codebase  
2. Use pattern matching like `find_all_pattern('function:has(call[text="console.log"])')`  
3. Extract parameter info with types  
4. Provide detailed analysis

## Technical Details

- Built on tree-sitter for correctness and performance  
- Includes 13 MCP tools for comprehensive code analysis  
- Supports JavaScript, TypeScript, JSX, TSX  
- Pattern parser converts CSS selectors to AST predicates  
- Stateful MCP server maintains analysis context

## Links

- [Library Repository](https://github.com/qckfx/tree-hugger-js)  
- [MCP Server Repository](https://github.com/qckfx/tree-hugger-js-mcp)  
- [NPM Package](https://www.npmjs.com/package/tree-hugger-js)  
- [Claude Code Integration](https://github.com/qckfx/tree-hugger-js-mcp#setup)

---

Would love feedback from the community, especially on the MCP integration!