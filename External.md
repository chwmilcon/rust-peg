# External Rules 
rust-peg allows for the inclusion of external rules within a grammar, enhancing modularity and reusability.

**Key Features:**

**Syntax:** External rules are invoked using the syntax `%%rulename()`.
**Scope:* These rules are not defined within the current grammar but are sourced from external libraries or modules.
Public Exposure: To enable external rule invocation, rust-peg makes public both the public functions `rulename()` and the internal `__parse_rulename()` functions.
**Benefits:**
**Modular Grammar Design:** Encourages the creation of reusable grammar components.
Library Integration: Facilitates the integration of pre-built grammar libraries.
Code Organization: Promotes cleaner and more maintainable grammar structures.

By exposing the internal __parse_rulename() functions, rust-peg provides flexibility for advanced usage scenarios, although this might introduce potential complexity and potential conflicts with other library components.
