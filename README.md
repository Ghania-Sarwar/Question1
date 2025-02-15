Queue-Based Path Conversion

Overview

This implementation converts a relative path to an absolute path using a queue-based approach. The method avoids built-in functions that directly convert paths, ensuring a manual approach to handling directory navigation.

How It Works

Current Directory Processing:

Splits the currentDir string by / and enqueues non-empty parts.
Code Structure

Queue

Implements Enqueue, Dequeue, and IsEmpty functions.

Conversion Function

Uses a Queue to process the absolute path manually

currentDir := "/home/user/docs"
relativePath := "../projects/code"
fmt.Println(conversion(currentDir, relativePath))
// Output: "/home/user/projects/code"
