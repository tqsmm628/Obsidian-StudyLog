---
subtitle: The Definitive Reference
status: doing
author: Joseph Albahari
publisher: O'Reilly
---
#book 
# Preface

## Intended Audience

## How This Book Is Organized

## What You Need to Use This Book

## Conventions Used in This Book

## Using Code Examples

## O'Reilly Online Learning

## How to Contact Us

## Acknowledgements

# Chapter 1. Introduction C# and .NET

## Object Orientation

### Unified type system

### Classes and interfaces

### Properties, methods, and events

### Functions can be treated as values

### C# supports patterns for purity

## Type Safety

## Memory Management

## Platform Support

## CLRs, BCLs, and Runtimes

### Common Language Runtime

### Base Class Library

### Runtimes

#### .NET 6

#### MAUI

#### UWP and WinUI 3

#### .NET Framework

### Niche Runtimes

## A Brief History of C#

### What's New in C# 10

#### File-scoped namespaces

#### The global using directive

#### Nondestructive mutation for anonymous types

#### New deconstruction syntax

#### Field initializers and parameterless constructors in structs

#### Record structs

#### Lambda expression enhancements

#### Nested property patterns

#### CallerArgumentExpression

#### Other new features

### What's New in C# 9.0

#### Top-level statements

#### Init-only setters

#### Records

#### Pattern-matching improvements

#### Target-typed new expressions

#### Interop improvements

#### Other new features

### What's New in C# 8.0

#### Indices and ranges

#### Null-coalescing assignment

#### Using declarations

#### Read-only members

#### Static local methods

#### Default interface members

#### Switch expressions

#### Tuple, positional, and property patterns

#### Nullable reference types

#### Asynchronous streams

### What's New in C# 7.x

#### C# 7.3

#### C# 7.2

#### C# 7.1

#### Numeric literal improvements

#### Out variables and discards

#### Type patterns and pattern variables

#### Local methods

#### More expression-bodied members

#### Deconstructors

#### Tuples

#### throw expressions

### What's New in C# 6.0

#### roslyn

#### null-conditional operator
#### Expression-bodied functions

#### Property initializers

#### Index initializers

#### String interpolation

#### Exception filters

#### using static directive

#### nameof()

### What's New in C# 5.0
#### async/await

### What's New in C# 4.0

#### Dynamic binding

#### Optional parameters

#### Type variance

#### COM interoperability

### What's New in C# 3.0

#### LINQ

#### Implicitly typed local variables

#### Object initializers

#### Lambda expressions

#### Extension methods

#### Query expressions

#### Expression trees

#### Automatic properties

#### Partial methods

### What's New in C# 2.0

#### Generics

#### nullable value types

#### iterators

#### anonymous methods

#### partial classes

#### static classes

# Chapter 2. C# Language Basics

## A First C# Program

### Compilation

## Syntax

### Identifiers and Keywords

#### Contextual keywords

### Literals, Punctuators, and Operators

### Comments

## Type Basics

### Predefined Type Examples

### Custom Types

#### Members of a type

#### Symmetry of predefined types and custom types

#### Constructors and instantiation

#### Instance versus static members

#### The public keyword

#### Defining namespaces

#### Defining a Main method

### Types and Conversions

### Value Types Versus Reference Types

#### Value types

#### Reference types

#### Null

#### Storage overhead

### Predefined Type Taxonomy

## Numeric Types

### Numeric Literals

#### Numeric literal type inference

#### Numeric suffixes

### Numeric Conversions

#### Converting between integral types

#### Converting between floating-point types

#### Converting between floating-point and integral types

#### Decimal conversions

### Arithmetic Operators

### Increment and Decrement Operators

### Specialized Operations on Integral Types

#### Division

#### Overflow

#### Overflow check operators

#### Overflow checking for constant expressions

#### Bitwise operators

### 8- and 16-Bit Integral Types

### Special Float and Double Values

### double Versus decimal

### Real Number Rounding Errors

## Boolean Type and Operators

### bool Conversions

### Equality and Comparison Operators

### Conditional Operators

#### Conditional operator (ternary operator)

## Strings and Characters

### Char Conversions

### String Type

#### String concatenation

#### String interpolation

#### String comparisons

#### Constant interpolated strings (C# 10)

## Arrays

### Default Element Initialization

#### Value types versus reference types

### Indices and Ranges

#### Indices

#### Ranges

### Multidimensional Arrays

#### Rectangular arrays

#### Jagged arrays

### Simplified Array Initialization Expressions

### Bounds Checking

## Variables and Parameters

### The Stack and the Heap

#### Stack

#### Heap

### Definite Assignment

### Default Values

### Parameters

#### Passing arguments by value

#### The ref modifier

#### The out modifier

#### Out variables and discards

#### Implication of passing by reference

#### The in modifier

#### The params modifier

#### Optional parameters

#### Named arguments

### Ref Locals

### Ref Returns

### var -- Implicitly Typed Local Variables

### Target-Typed new Expressions

## Expressions and Operators

### Primary Expressions

### Void Expressions

### Assignment Expressions

### Operator Precedence and Associativity

#### Precedence

#### Left-associative operators

#### Right-associative operators

### Operator Table

## Null Operators

### Null-Coalescing Operator

### Null-Coalescing Assignment Operator

### Null-Conditional Operator

## Statements

### Declaration Statements

### Local variables

### Expression Statements

### Selection Statements

#### The if statement

#### The else clause

#### Changing the flow of execution with braces

#### The switch statement

#### Switching on types

#### Switch expressions

### Iteration Statements

#### while and do-while loops

#### for loops

#### foreach loops

### Jump Statements

#### The break statement

#### The continue statement

#### The goto statement

#### The return statement

#### The throw statement

### Miscellaneous Statements

## Namespaces

### File-Scoped Namespaces (C# 10)

### The using Directive

### The global using Directive (C# 10)

#### Implicit global using

### using static

### Rules Within a Namespace

#### Name scoping

#### Name hiding

#### Repeated namespaces

#### Nested using directives

### Aliasing Types and Namespaces

### Advanced Namespace Features

#### Extern

#### Namespace alias qualifiers

# Chapter 3. Creating Types in C\#

## Classes

### Fields

#### The readonly modifier

#### Field initialization

#### Declaring multiple fields together

### Constants

### Methods

#### Expression-bodied methods

#### Local methods

#### Static local methods

#### Local methods and top-level statements

#### Overloading methods

### Instance Constructors

#### Overloading constructors

#### Implicit parameterless constructors

#### Constructor and field initialization order

#### Nonpublic constructors

### Deconstructors

### Object Initializers

#### The this Reference

### Properties

#### Read-only and calculated properties

#### Expression-bodied properties

#### Automatic properties

#### Property initializers

#### get and set accessibility

#### Init-only setters

#### CLR property implementation

### Indexers

#### Implementing an indexer

#### CLR indexer implementation

#### Using indices and ranges with indexers

### Static Constructors

#### Static constructors and field initialization order

### Static Classes

### Finalizers

### Partial Types and Methods

#### Partial methods

#### Extended partial methods

### The nameof operator

## Inheritance

### Polymorphism

