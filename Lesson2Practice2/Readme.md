# Exploring Generic Variables

In this practice session, I have explored the Generic Variable type avaiable under UiPath.Core.

## Key Concept
The first element in your expression is used as a guideline for what operation Studio performs. For example, when you try to add two GenericValue variables, 
if the first one in the expression is defined as a String, the result is the concatenation of the two. If it is defined as an Integer, 
the result is their sum.

## Getting Started
Download the file or clone in to your local machine and open it through the UiPath Community edition.
No additional packages required.

## Problem Statement
Create four variables of the GenericValue type in your sequence. Print to the console various operations with them and observe the result.

## Example
Adding two Strings together is called concatenation. For example, when we concatenate “cat”+”dog”, the result is “catdog”. 
The same happens when two GenericValue variables are added together. For instance, “123”+123 becomes “123123” with string concatenation, 
but 123+“123” becomes 246 with regular integer addition.


