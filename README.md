# TypeScript Strict Null Checks and undefined

This example demonstrates a common issue encountered when using TypeScript's strict null checks.  The `printName` function is designed to handle null values gracefully, but it throws an error when called with `undefined`.  This is because, in TypeScript, `undefined` and `null` are distinct types, and `undefined` is not a subtype of `null`.

The solution involves adjusting the function's type definition to accommodate both `null` and `undefined`.