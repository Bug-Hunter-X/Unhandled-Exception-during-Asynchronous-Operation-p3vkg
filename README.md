# Unhandled Exception during Asynchronous Operation in Dart

This example demonstrates a common error in Dart code involving asynchronous operations and exception handling. The `fetchData` function attempts to fetch data from a remote API. While it includes a `try-catch` block, it doesn't comprehensively handle all possible exceptions that might occur during the process.

Specifically, the `jsonDecode` function can throw a `FormatException` if the API response isn't valid JSON. The code also lacks specific error handling for network issues. 

The solution demonstrates how to improve this by adding specific exception handling for `FormatException` and using a more robust approach to handle network errors.