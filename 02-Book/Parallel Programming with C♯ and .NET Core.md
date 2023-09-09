---
subtitle: Developing Multithreaded Applicatioins Using C# and .NET Core 3.1 from Scratch
status: doing
author: Rishabh Verma, Neha Shrivastava, Ravindra Akella
publisher: bpb
---
#book 
# 1. Getting Started

## Structure

## Objective

## Download essential tools for Windows

## Installing Visual Studio 2019 with .NET Core 3.1

## Perfmon

## Procmon

## Process Explorer

## PerfView

## JustDecompile

## DebugDiag

## WinDbg

## Creating a .NET Core 3.1 application using Visual Studio 2019

## Summary

## Exercise

# 2. What's New in C# 8

## Structure

## Objective

## C# 8 platform dependencies

## New features and enhancements

### Nullable reference types/Non-nullable reference type

### Asynchronous streams

### Ranges and indices

#### System.Index

#### System.Range

## Default implementations of interface members

## Readonly members on structs

## Pattern matching enhancements

### Switch expressions

#### Recursive patterns

#### Positional pattern

#### Property pattern

### Tuple patterns

## Using declarations

## Static local functions

## Disposable ref structs

## Null-coalescing assignment

## Interpolated verbatim strings enhancement

## Summary

## Exercise

# 3. .NET Core 3.1

## Introduction

## Structure

## Objective

## New features and enhancements

## NET Core version APIs

## Windows Desktop application support

### Windows Desktop Deployment MSIX

## COM-callable components - Windows Desktop

## WinForms high DPI

## .NET Standard 2.1

## C# 8 and its new features support

## Compile and Deploy

### Default executable

### Single executable file

### Assembly linking

### Tiered compilation

### ReadyToRun images

### Cross-platform/architecture restrictions

## Runtime/SDK

### Build copies dependencies

### Local tools

### Smaller Garbage Collection heap sizes

### Garbage Collection Large Page supports

### Opt-in feature

## IEEE Floating-point improvements

## Built-in JSON support

### Json Reader

### Json Writer

### Json Serializer

## HTTP/2 support

## Cryptographic Key Import and Export

## Summary

## Exercise

# 4. Demystifying Threading

## Structure

## Objectives

## Why threading?

### Developing a responsive user interface

### Handling concurrent requests in server

### Leverage the full power of the multi-core computing

### Improving performance by proactive computing

## What is threading?

## Thread

## Exception handling

### Limitations

## ThreadPool

### Exceptions in ThreadPool

### Limitations of Thread Pool

## ThreadPool in action

## Task

## TaskCreationOptions

## Exception handling with Tasks

## Cancellation

## Continuations

## WhenAll, WhenAny

## Task Scheduler

## Task Factory

## Summary

## Exercise

# 5. Parallel Programming

## Structure

## Objectives

## Understanding the jargon

## Parallel Extensions

## Task Parallel Library (TPL)

## Data parallelism

## Task parallelism

### PLINQ

## Data structures for parallelism

### ConcurrentBag\<T>

### ConcurrentStack\<T>

### ConcurrentQueue\<T>

### ConcurrentDictionary\<TKey, TValue>

## IEnumerator and yield return

## async await

## async await - Control flow

## async await - Under the hood

### Language features

## Principles for using async await

## Restrictions on async await

### CPU (computer) bound versus I/O bound word

## Deadlock

## Asynchronous Streams

## ValueTask

## Summary

## Exercise

# 6. The Threading Patterns

## Introduction

## Structure

## Objectives

## Task-based Asynchronous Pattern (TAP)

### Implementing pattern

### CPU bound versus I/O bound

### Exception handling

#### Nested exception handling

#### Exception handling in Task.Wait()

#### Using the handle method

### Avoid async void

### Cancellation

### Progress reporting

### Other asynchronous patterns

## Asynchronous Programming Model (APM)

### APM to TAP wrapper

### TAP to APM wrapper

## Event-based Asynchronous Pattern (EAP)

### EAP to TAP wrapper

## Summary

## Exercise

# 7. Synchronization Constructs

## Structure

## Objectives

## Overview

### Thread safety

## Locking constructs

### Lock or Monitor.Enter/Monitor.Exit (Exclusive)

### Mutex (Exclusive)

### SpinLock (Exclusive)

### Semaphore (Non-Exclusive)

### SemaphoreSlim (Non-Exclusive)

### Reader/Writer locks (Non-Exclusive)

## Signaling constructs

### AutoResetEvent

### ManualResetEvent / ManualResetEventSlim

### CountdownEvent

### Barrier classes

### Wait and Pulse

### Interlocked class

### Volatile class

## Summary

## Exercise

# 8. Unit Testing Parallel and Asynchronous Programs

## Structure

## Objectives

## Overview

## Basics of unit testing with XUnit

### Executing unit tests

### IntelliTest

### Live Unit Testing

### Unit test async methods

### Unit test exceptions in async methods

### Unit test async method using mock data

## Unit test for parallel methods

### Unit test async void methods

## Summary

## Exercise

# 9. Debugging and Troubleshooting

## Structure

## Objectives

## Debugging primer with Visual Studio 2019

## Profiling

## Memory Dumps

### Collecting memory dumps

