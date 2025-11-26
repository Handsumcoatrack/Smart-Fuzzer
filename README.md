# Fuzzer-tool
This tool will be used to test a programs weaknesses and report back to see where it fails.
--

# New added Features are listed by catagory below
---
# Performance

Connection pooling (reuses TCP connections via requests.Session())
Multi-threading (concurrent requests using thread pools)
Configurable delay / rate limiting (prevents getting blocked)

# Detection

Content matching (search responses for specific strings or regex patterns)
Exclusion filters (ignore responses containing certain content)
Baseline comparison (detects anomalies by comparing against "normal" 404 responses)

# Flexibility

Multiple injection points (FUZZ, FUZZ2, FUZZ3, FUZZ4 with separate wordlists)
Multiple HTTP methods (GET, POST, PUT, DELETE)
POST data fuzzing
Custom header injection
Cookie support

# Robustness

Error handling (catches timeouts, connection errors, SSL errors, etc.)
Retry logic with exponential backoff (retries failed requests with increasing wait times)
Input validation (checks for FUZZ placeholder, tests connectivity before starting)

# Usability

Argument parsing with argparse (clean command-line interface with named flags)
Help menu (--help shows all options with examples)
Summary output (shows findings, errors, and anomalies at the end)
