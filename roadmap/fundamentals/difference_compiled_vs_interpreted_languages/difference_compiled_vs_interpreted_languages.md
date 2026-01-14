## Compiled vs. Interpreted Programming Languages

**Translations**

- [EN-US](./difference_compiled_vs_interpreted_languages.md)
- [PT-BR](./pt_br/diferenca_linguagens_compiladas_vs_interpretadas.md)

## Navigation
<details>
<summary><b>Menu</b></summary>

- [Introduction](#introduction)
- [Types of Programming Languages](#types-of-programming-languages)
- [Breaking the Problem into Parts](#breaking-the-problem-into-parts)
  - [Part 1](#part-1)
  - [Part 2](#part-2)
  - [Conclusion of the Problem](#conclusion-of-the-problem)
- [How They Work](#how-they-work)
    - [Compiled Languages](#compiled-languages)
    - [Interpreted Languages](#interpreted-languages)
- [Comparative Table](#comparative-table)
- [Credits](#credits)
</details>

<br />

# Introduction

In the world of computers, all programming languages are simply instructions that sooner or later become Hexadecimals or Binaries, and we will explore this further soon. You might be wondering, where are you going with this?

The answer is quite simple: in this lesson, you will learn the difference between compiled programming languages and interpreted programming languages.

# Types of Programming Languages

Programming languages up until now are divided into two types:

- Compiled Languages.
- Interpreted Languages.

Don't worry, we will go into the details of the differences between them with some examples from an external perspective.

Like everything in a computer, from the hardware to how technologies work, it all starts with something that humans have a deep knowledge and experience with. Programming languages are no different.

# Breaking the Problem into Parts
## Part 1

**1.** Let’s imagine a hypothetical scenario where you have a manual for installing a new tool that you will start using in your daily work routine;<br />
**2.** You are in Japan, and in this hypothetical example, you do not speak, read, or write Japanese;<br />
**3.** You need to be able to correctly install the software;<br />
**4.** You do not live in a technological world with smartphones, cell towers supporting technologies like 3G, 4G, 5G, or any other internet resources such as Wi-Fi, Hotspot, etc.
<br /><br />

## Part 2

Knowing this, you have a few alternatives left, which are:

**A)** If there is a department responsible for translations within the company, they would take care of translating the installation manual from Japanese to your native language;<br />
**B)** If you have a friend who speaks and reads Japanese, they can sit next to you during the installation process and translate line by line in real-time for you.
<br /><br />

## Conclusion of the Problem

In option **A**, you have someone who translates everything to your native language so that things can be executed, and this is equivalent to a **Compiled Language**.

On the other hand, in option **B**, you have a person who interprets everything that is written and translates it step by step for you, and this is equivalent to an **Interpreted Language**.
<br /><br />

# How They Work

### Compiled Languages

Compiled languages work by converting the instructions written in English by programmers, developers, and software engineers into machine language, also known as **Binary Language** or **Binary System**. This, not by coincidence, is the language that your processor (CPU) uses to communicate with all the parts (hardware pieces) and systems within your computer.

Another feature of compiled languages is that precisely because they convert English text instructions into code that is understandable and readable by the machine, these languages require a step called **Building**, where the **Compiler** reads all the English instructions and then converts them into binary numbers for the processor. They also give developers more control over certain aspects of the hardware, such as memory management and CPU usage.

During this Building step, your instructions written in English are converted into a file called `Binaries`, which will later be more easily understood by the computer when it needs to execute that program. After all, the program will have already been converted into something that is in the computer's native language. Usually, your code is converted into files with extensions like `.exe` (Windows), `.app` (macOS), `.dll` (Windows), `.kext` (macOS), among others.

And precisely because of the Building step, languages tend to be faster for developing heavy applications, such as games, operating systems, and other high-performance applications.
<br /><br />

### Interpreted Languages

Interpreted languages, on the other hand, mostly work through a technology called [JIT Compilation](https://en.wikipedia.org/wiki/Just-in-time_compilation) (Just In Time Compilation), or Dynamic Compilation, which is briefly a method to enhance the performance of interpreted languages by compiling the program into native code during execution to improve its performance and response time.

If the big difference between compiled and interpreted languages is not yet clear, here's a big hint. Interpreted languages go through the code of a program line by line, executing each command. One important detail is that a language as a whole is not necessarily 100% interpreted. There are cases, like the Python language, for example, which, despite being considered an interpreted language, has C acting on its lower layer to compile certain information quickly.
<br /><br />
<br /><br />

# Comparative Table
<br /><br />

| **Criteria** | **Compiled Languages** | **Interpreted Languages** |
|:--:|:--:|:--:|
| **Building** | Requires a building step. The compiler reads the entire code and converts it into a binary file that is sent to the CPU for execution. | Does not necessarily require building for all functionalities. Code snippets are compiled dynamically by an interpreter and sent to the CPU for execution. |
| **How It Works** | Relies on a compiler to compile the code. | In most cases, does not depend on a compiler to execute the code. |
| **Syntax Analysis** | Analyzes code errors beforehand and prevents the conversion of the programming language into machine code (binary) if errors are found. | Does not analyze errors beforehand; executes the code first and reports errors during execution. |
| **Performance Speed** | Generally offers better performance and speed by communicating directly with the machine after being converted into binary. | Has lower performance and speed, but allows the source code to be modified during runtime. Exceptions exist, such as Python using C for performance-critical operations. |
| **Memory Management Capability** | Greater control over memory manipulation through pointers, pointer arithmetic, and manual memory allocation and deallocation. | Less flexible when it comes to direct memory manipulation. |
| **Languages** | Assembly, B, BASIC, C, C++, C#, Delphi, Fortran, Go, Java, Pascal, Rust, Visual Basic | Bash, CoreSE, JavaScript, Lua, Perl, PHP, Python, R, Ruby |
| **Usage** | Operating Systems, Games, Embedded Systems, Cloud Systems, IoT Systems | Data Science, Machine Learning, Applications, Artificial Intelligence, Data Analysis |

<br />

# Credits

| [<img src="https://github.com/sdkitagawa.png?size=50" width=50><br /><sub>@sdkitagawa</sub>](https://github.com/sdkitagawa) |
| :---: |
