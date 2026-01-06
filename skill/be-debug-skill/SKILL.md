# Backend Debugging Skills – TypeScript / Go / Rust

## 🧠 Debugging Mindset

* Systematic root-cause analysis
* Reproduce bugs from real execution paths
* Separate data issues from logic issues
* Prefer observability over assumptions
* Debug behavior, not just code

---

## 🧩 Backend Logic Debugging

* Trace business logic across multiple layers
* Validate assumptions in domain logic
* Detect incorrect state transitions
* Debug edge cases & invalid input handling
* Identify silent failures & swallowed errors

---

## 🔍 Runtime & Execution Debug

* Step-through debugging
* Inspect call stacks & execution flow
* Debug async / concurrent execution
* Identify blocking, deadlocks & race conditions
* Analyze unexpected panics / crashes

---

## 📊 Data & State Debugging

* Debug inconsistent state between services
* Validate database writes & reads
* Handle eventual consistency issues
* Detect stale cache & invalidation bugs
* Compare expected vs actual data state

---

## 🌐 API & Service Debugging

* Debug REST / GraphQL service behavior
* Request / response lifecycle tracing
* Debug malformed payloads & schema mismatches
* Authentication & authorization logic debugging
* Validate idempotency & retry behavior

---

## 🧵 Concurrency & Async Debug

* Debug async execution flow
* Race condition detection
* Locking & synchronization issues
* Goroutine / async task lifecycle debugging
* Backpressure & queue saturation analysis

---

## 🧪 Testing-Oriented Debug

* Reproduce bugs via unit & integration tests
* Write minimal test cases to isolate logic
* Debug flaky tests
* Property-based testing awareness
* Regression prevention through tests

---

## 🧾 Logging & Observability

* Structured logging design
* Log correlation across services
* Use logs to reconstruct execution flow
* Avoid noisy logs, focus on signal
* Debug via metrics & traces

---

## 🛠 Language-Specific Debug Skills

### TypeScript / Node.js

* Debug async/await & promise chains
* Event loop & task queue understanding
* Memory leak detection
* Runtime type mismatch debugging
* Validate runtime vs compile-time assumptions

---

### Go

* Debug goroutines & channels
* Identify deadlocks & race conditions
* Panic & recover analysis
* Context propagation debugging
* Memory & GC behavior awareness

---

### Rust

* Debug ownership & borrowing issues
* Lifetime-related logic errors
* Result / Option misuse detection
* Async runtime debugging (Tokio)
* Safe vs unsafe code boundary awareness

---

## 🧱 Infrastructure-Aware Debug

* Debug environment-specific issues
* Configuration & secret mismatch detection
* Dependency version conflicts
* Startup & initialization order bugs
* Resource exhaustion issues (CPU, memory, file descriptors)

---

## 🔁 Cross-Service Debug Workflow

* Trace requests across service boundaries
* Correlate logs using request IDs
* Identify failure propagation paths
* Debug partial failures in distributed systems
* Write clear incident timelines

---

## 🧠 Engineering Principles

* Fail fast with explicit errors
* Defensive programming
* Make invalid states unrepresentable
* Prefer clarity over cleverness
* Optimize for debuggability

---

## 🎯 Debugging Focus

* Business logic correctness
* Data integrity & consistency
* Predictable system behavior
* Reliability under load
* Maintainability & long-term stability
