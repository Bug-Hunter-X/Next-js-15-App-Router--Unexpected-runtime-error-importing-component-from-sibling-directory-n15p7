# Next.js 15 App Router: Unexpected runtime error importing component from sibling directory

This repository demonstrates a runtime error encountered when importing a component from a sibling directory within the Next.js 15 App Router.  The error arises seemingly without any clear build-time warnings.

## Bug Report

The `bug.js` file contains a simple Next.js app directory setup.  It attempts to import a component `MyComponent` from the same directory. This results in an unexpected runtime error.

## Solution

The `bugSolution.js` illustrates the resolution. The problem is resolved by using a relative path with leading `./` to resolve the import path correctly.