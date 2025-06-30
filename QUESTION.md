# 🧠 Senior Golang Coding Challenge: Concurrent Log Analyzer

Welcome! This coding challenge tests your ability to build scalable, concurrent, and idiomatic systems in Go. The focus is on concurrency, file handling, data aggregation, and clean architecture.

---

## 🚀 Problem Statement

Build a **log file analyzer** in Go that concurrently processes multiple large log files and extracts **error statistics**.

---

## 🔧 Requirements

Your Go program should:

1. Accept a list of **log file paths**
2. **Concurrently** read and parse each log file using goroutines
3. Extract and aggregate:
   - Total number of lines
   - Number of `INFO`, `WARN`, and `ERROR` entries
   - The most frequent error message
4. Handle errors gracefully (e.g., unreadable files, malformed lines)

---

## 📘 Sample Log Format

Each log line will follow this format:
```
2025-06-30T10:15:00Z [INFO] Starting service
2025-06-30T10:16:12Z [WARN] Memory usage high
2025-06-30T10:17:45Z [ERROR] Connection timeout
```

---

## 📦 Sample Output

```bash
Log Summary:
Files processed: 3
Total lines: 350000
INFO: 220000
WARN: 90000
ERROR: 40000
Most common error: "Connection timeout"
```

---

## 🧪 Bonus Points (Optional)

- ✅ Add **unit tests** for your logic
- ✅ Support **streaming input** (e.g., stdin or HTTP uploads)
- ✅ Use **channels** for fan-in result aggregation
- ✅ Make output configurable (stdout or report file)
- ✅ Design it to be extensible (e.g., for JSON log format)

---

## ✅ Evaluation Criteria

- Efficient, idiomatic Go
- Proper use of goroutines, channels, and worker pool
- Concurrency safety and performance
- Robust error handling
- Clean architecture and structure
- Unit test coverage

---

## 📁 Submission Guidelines

- Include all your code in a directory `/loganalyzer`
- Include a `main.go` to demonstrate usage
- Add any test files with the `_test.go` suffix
- Include a short note if anything needs explanation
- Ensure the solution builds and runs with Go 1.20+

---

## 🙋‍♂️ Questions?

Feel free to leave a comment if anything is unclear.  
Good luck — and happy coding! 🚀
