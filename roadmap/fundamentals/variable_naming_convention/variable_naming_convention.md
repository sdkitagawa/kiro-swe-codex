## Variable Naming Convention

**Translations**

- [EN-US](./variable_naming_convention.md)
- [PT-BR](./pt_br/convencao_de_nomenclatura_de_variaveis.md)

## Navigation
<details>
<summary><b>Menu</b></summary>

- [How to Properly Name Variables](#how-to-properly-name-variables)
  - [Be descriptive and meaningful](#be-descriptive-and-meaningful)
  - [Use consistent casing conventions](#use-consistent-casing-conventions)
  - [Avoid single-letter names (except in limited scopes)](#avoid-single-letter-names-except-in-limited-scopes)
  - [Do not use abbreviations unless they are well-known](#do-not-use-abbreviations-unless-they-are-well-known)
  - [Reflect the data type or intent when helpful](#reflect-the-data-type-or-intent-when-helpful)
  - [Keep names concise but not cryptic](#keep-names-concise-but-not-cryptic)
  - [Use positive names for booleans](#use-positive-names-for-booleans)
  - [Avoid reserved words and misleading names](#avoid-reserved-words-and-misleading-names)
  - [Maintain consistency across the codebase](#maintain-consistency-across-the-codebase)
  - [Name variables based on what they represent, not how they are used](#name-variables-based-on-what-they-represent-not-how-they-are-used)
  - [Avoid overly generic names](#avoid-overly-generic-names)
  - [Use domain-specific terminology](#use-domain-specific-terminology)
  - [Rename variables when their purpose changes](#rename-variables-when-their-purpose-changes)
  - [Favor readability over personal preference](#favor-readability-over-personal-preference)
- [Credits](#credits)
</details>

<br />

# How to Properly Name Variables

## Be descriptive and meaningful

- Use names that clearly explain the variable’s purpose (e.g., `userName` instead of `usr`).

## Use consistent casing conventions

- `camelCase` for most variables (common in JavaScript, Java, Python, C/C++).
- `snake_case` for languages like Python where it’s idiomatic.
- `PascalCase` typically reserved for classes, not variables.

> The convention may change according to project standards.

## Avoid single-letter names (except in limited scopes)

- Acceptable in loops (`i`, `j`, `k`...) or mathematical contexts, but not for general variables.

## Do not use abbreviations unless they are well-known

- Prefer `maximumLength` over `maxLen` unless the abbreviation is widely understood.

## Reflect the data type or intent when helpful

- Use plural nouns for collections: `users`, `itemsList`.
- Use boolean prefixes like `is`, `has`, or `can`: `isActive`, `hasPermission`.

Avoid encoding type information unnecessarily

- Do not use prefixes like `strName` or `intCount` unless the language or project requires it.

## Keep names concise but not cryptic

- Balance readability and brevity (`errorMessage` is better than `detailedErrorMessageForUserInput`).

## Use positive names for booleans

- Prefer `isEnabled` over `isNotDisabled` to reduce mental overhead.

## Avoid reserved words and misleading names

- Do not shadow built-in functions or keywords, e.g.: `list`, `string`, `class`.

## Maintain consistency across the codebase

- Choose one naming style and apply it everywhere to improve readability.

## Name variables based on what they represent, not how they are used

- Focus on the concept `userAge` rather than the computation `currentYearMinusBirthYear`.

## Avoid overly generic names

- Names like `data`, `value`, or `temp` should be used only when their meaning is truly obvious.

## Use domain-specific terminology

- Align variable names with the business or problem domain to improve clarity.

## Rename variables when their purpose changes

- If a variable evolves, update its name to reflect its new responsibility.

## Favor readability over personal preference

- Choose names that make sense to the entire team, not just the author.

<br />

# Credits

| [<img src="https://github.com/sdkitagawa.png?size=50" width=50><br /><sub>@sdkitagawa</sub>](https://github.com/sdkitagawa) |
| :---: |
