# React Native: Handling Invalid URLs in Fetch Requests

This repository demonstrates a common error in React Native applications: crashing due to an invalid URL in a `fetch` request.  The original code uses an invalid URL which causes the app to crash. The solution demonstrates robust error handling to gracefully handle such situations.

## Problem

The application attempts to fetch data from an invalid URL.  If the fetch fails, the app crashes instead of displaying an appropriate error message to the user.

## Solution

The improved code incorporates comprehensive error handling within the `try...catch` block. The `finally` block ensures that the loading indicator is always hidden, regardless of whether the fetch was successful or not.  Even if the response isn't okay (e.g., a 404), the application handles this without crashing, providing informative error feedback to the user.