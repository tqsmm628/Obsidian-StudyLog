---
status: doing
author: Jort Rodenburg
publisher: manning
---
#book
# Part 1 Using C# and .NET

## 2 .NET and how it compiles

### 2.1 What is the .NET Framework

### 2.2 What is .NET 5?

### 2.3 How CLI-compliant languages are compiled

#### 2.3.1 Step 1: C# code (high-level)

#### 2.3.2 Step 2: Common Intermediate Language (assembly level)

#### 2.3.3 Step 3: Native code (processor level)

### Summary

# Part 2 The existing codebase

## 3 How bad is this code?

### 3.1 Introducing Flying Dutchman Airlines

### 3.2 Pieces of the puzzle: Taking a look at our requirements

#### 3.2.1 Object-relation mapping

#### 3.2.2 The GET /flight endpoint: Retrieving information on all flights

#### 3.2.3 The GET /flight/{flightNumber} endpoint: Getting specific flight information

#### 3.2.4 The POST /booking/{flightNumber} endpoint: Booking a flight

### 3.3 Coming to terms with the existing codebase

#### 3.3.1 Assessing the existing database schema and its tables

#### 3.3.2 The existing codebase: Web service configuration files

#### 3.3.3 Considering models and views in the existing codebase

### Summary

## 4 Manage your unmanaged resources!

### 4.1 The FlightController: Assessing the GET /flight endpoint

#### 4.1.1 The GET /flight endpoint and what it does

#### 4.1.2 Method signature: The meaning of ResponseType and typeof

#### 4.1.3 Collecting flight information with collections

#### 4.1.4 Connection strings, or how to give a security engineer a heart attack

#### 4.1.5 Using IDisposable to release unmanaged resources

####  4.1.6 Querying a database with SqlCommand

### 4.2 The FlightController: Assessing GET /flight/{flightNumber}

### 4.3 The FlightController: POST /flight

