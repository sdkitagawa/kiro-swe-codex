## Typing and Types of Languages

**Translations**

- [EN-US](./strong_vs_weak_typing_and_dynamic_vs_stactic_languages.md)
- [PT-BR](./pt_br/linguagens_fortemente_vs_fracamente_tipadas_e_dinamicas_vs_estaticas.md)

## Navigation
<details>
<summary><b>Menu</b></summary>

- [Introduction](#introduction)
- [What is typing?](#what-is-typing)
- [Typing in Parts](#typing-in-parts)
    - [Strong Typing](#strong-typing)
    - [Weak Typing](#weak-typing)
    - [Static Languages](#static-languages)
    - [Dynamic Languages](#dynamic-languages)
- [Bindings and Differences](#bindings-and-differences)
    - [Static and Strong Typing](#static-and-strong-typing)
    - [Static and Weak Typing](#static-and-weak-typing)
    - [Dynamic and Strong Typing](#dynamic-and-strong-typing)
    - [Dynamic and Weak Typing](#dynamic-and-weak-typing)
- [Languages and Their Types](#languages-and-their-types)
- [Credits](#credits)
</details>

<br />

# Introduction
When studying programming and development, it is inevitable that sooner or later you will come across terms like "strong" typing, "weak" typing, and "static" or "dynamic" languages. You will also find a variety of discussions around which language is which and why.

In this lesson, we will unravel the mysteries behind this complicated and much-discussed topic.
<br /><br />

# What is typing?
Typing is what determines whether your language will be slower, more dynamic, with a lower barrier to entry for learning and working, or if it will be faster, static, with a higher barrier to entry for learning and working.

Believe me, I know, there is a dilemma here. After all, why spend more time studying a complex programming language to enter the job market, when by studying a simpler language I could learn to program faster and enter the market sooner?

Although it may be tempting to think this way, my job as a good teacher and mentor is to open your eyes to the reality and clarify as soon as possible that when we talk about typing, it doesn't always involve the language with the least barrier to entry or the least complexity in learning, or the opposite.

When we talk about typing, we need to consider a number of factors, such as:

- How much you will really be learning about the essential fundamentals to truly understand what you are doing, like why things happen the way they do, and what the origins of the technologies available to us are;

- Whether it's worth focusing on languages like **JavaScript**, **Perl**, and **PHP** which, due to their **weak typing**, provide you with _more agility_ due to the _lack of data typing_, more freedom to develop something without worrying too much about _system design_, _simpler syntax_, _lower learning curve_ for beginners, etc. However, later on, you will _spend more time_ dealing with a higher number of _bugs that appear during runtime_ precisely because of the lack of strong typing, which will cause future problems in applications that grow and scale more than expected. This will force you and your team to put a tremendous effort into creating [unit tests](https://aws.amazon.com/what-is/unit-testing/), [linters](https://www.testim.io/blog/what-is-a-linter-heres-a-definition-and-quick-start-guide/), [CI/CD (Continuous Integration/Continuous Delivery)](https://about.gitlab.com/topics/ci-cd/) etc.;

- Maybe it’s worth focusing on languages like **C#** and **Java** which, due to their **strong typing**, provide you with _greater security_ in development, since _fewer bugs occur during runtime_. You also pay _more attention to your system's design_ from the early stages of development. But in the end, you have a steeper learning curve for beginners, and it makes you _lose agility and time_ having to constantly infer types correctly, understand the complexity of types, and work with a lot of [boilerplate code](https://aws.amazon.com/what-is/boilerplate-code/#:~:text=Boilerplate%20code%20is%20computer%20language,minimal%20changes%20for%20different%20situations.);

That said, without further ado, let's dive into the more direct explanations.
<br /><br />

# Typing in Parts
### Strong Typing
- Variables, in most cases, cannot be **null**;
- Variables must have a type;
- Variables must be initialized;
- Variables cannot have their type changed after being declared.
<br /><br />

### Weak Typing
- Variables can be **null**;
- Variables do not require a type, as the language itself determines the type based on the data stored in it;
- Variables do not necessarily need to be initialized (but may be, if necessary);
- Variables can have their type changed even after being declared.
<br /><br />

### Static Languages

Static languages do not allow you to change the variable type after it is declared.

- Anti-Dynamism;
  - The language is compiled;
  - You get real-time feedback on your code through your IDE (within your code editor);
  - Better performance at runtime;
  - Provides more security;
  - Errors are detected more quickly (_redundant with point 2, but still worth mentioning_);
  - A slower prototyping process;
  - They are best for developing games, security-related applications, embedded systems (systems typically developed for machines and robots), operating systems, firmware (micro-operating systems typically developed for handheld consoles, modems, routers, cable TV transmission devices).
<br /><br />

### Dynamic Languages

Dynamic languages are linked to the ability to allow the same variable to hold values of different types during code execution.

- Dynamism;
  - The language is interpreted;
  - You do not get real-time feedback on your code through your IDE (within your code editor) without using linters;
  - Worse performance and execution time;
  - Lower security;
  - Faster prototyping process;
  - They are best for backend systems for websites, backend systems for apps, neural networks (artificial intelligence), video and image rendering through code, quantum/complex calculations (weather systems, time, and other utilities involving physics).
<br /><br />

# Bindings and Differences
### Static and Strong Typing
Static and strong typing languages provide the following features:

- Type checking at compile-time;
- Explicit type inference;
  - Forcing the developer to always specify the variable type;
- Fewer implicit conversions.
  - When working with two incompatible data types, like a `string` and an `integer`, you cannot perform an addition with them. Therefore, you cannot simply convert one value to the other, requiring the use of Casts and Parsers to transform the types.
<br /><br />

### Static and Weak Typing
Static and weak typing languages, on the other hand, provide:

- Type checking at compile-time;
- Implicit type conversions;
  - You can convert data types with fewer difficulties.
<br /><br />

### Dynamic and Strong Typing
Dynamic and strong typing languages provide:

- No permission for operations between different types without explicit conversion;
- No permission for automatic ("magical") operations between incompatible types.
<br /><br />

### Dynamic and Weak Typing
Dynamic and weak typing languages provide:

- Flexibility of types;
  - For example, adding an `integer` type with a `string` and having the result be an `integer`.
- Automatic ("magical") type conversions.
<br /><br />

# Languages and Their Types
Reading method for the table:
- Read starting from the **Y-axis** (top to bottom) vertically;
- Then read the **X-axis** (left to right) horizontally.

| **Intensity** | **Static** | **Dynamic** |
|:--:|:--:|:--:|
| **Strong** | C#, Dart, Delphi, F#, Haskell, Java, Kotlin, Pascal, Rust, Scala, Swift | Clojure, Erlang, Groovy, Lua, Python, Ruby, TypeScript |
| **Weak** | C, C++, C--, C*, COBOL | CoreSE, JavaScript, Perl, PHP, Visual Basic |

# Credits

| [<img src="https://github.com/sdkitagawa.png?size=50" width=50><br /><sub>@sdkitagawa</sub>](https://github.com/sdkitagawa) |
| :---: |
