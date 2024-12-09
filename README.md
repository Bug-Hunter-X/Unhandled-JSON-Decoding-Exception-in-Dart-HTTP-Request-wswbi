# Unhandled JSON Decoding Exception in Dart

This repository demonstrates a common error in Dart applications involving handling HTTP responses and JSON decoding. The original code lacks proper error handling for invalid JSON data, leading to unexpected crashes. The solution provides a more robust approach.

## Bug

The `bug.dart` file shows the original code with inadequate error handling.  `jsonDecode` is used without sufficient checks for invalid JSON responses, potentially causing runtime exceptions.

## Solution

The improved code in `bugSolution.dart` addresses the issue by using a `try-catch` block specifically for `FormatException` thrown by `jsonDecode`. This handles invalid JSON responses gracefully without crashing the app, providing more informative error messages.