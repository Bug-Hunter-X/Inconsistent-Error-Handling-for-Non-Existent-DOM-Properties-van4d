# Inconsistent Error Handling for Non-Existent DOM Properties

This repository demonstrates a subtle bug related to accessing non-existent properties of DOM elements in HTML.  The issue lies in the inconsistent error handling across different browsers and versions.

## Description

The `bug.html` file contains a script that attempts to access a property (`nonExistentProperty`) that does not exist on the `myDiv` element.  While some modern browsers might throw a `TypeError`, others might not, leading to unpredictable behavior or silent failures.

The `solution.html` file provides a corrected version, using an optional chaining operator or checking for the property's existence before access.

## How to Reproduce

1. Clone this repository.
2. Open `bug.html` in different web browsers (e.g., Chrome, Firefox, Safari, Edge).
3. Observe the behavior; some browsers may throw errors, while others might not.
4. Open `solution.html` to see the corrected approach.

## Solution

The solution demonstrates how to prevent this issue by checking for property existence or using optional chaining.