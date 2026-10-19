## Charles Proxy to Postman

### Objective
Demonstrate the ability to capture HTTP requests using Charles Proxy, reproduce them in Postman, and validate responses through automated assertions.

### Test Scenarios

| Scenario | Charles Capture | Postman Evidence | Validation |
|---|---|---|---|
| GET a single post | `evidence/charles/01-charles-get-post.png` | `evidence/postman/01-postman-run-results-1.png` | HTTP 200 and response structure |
| GET posts filtered by user | `evidence/charles/02-charles-get-filtered-posts.png` | `evidence/postman/02-postman-run-results-2.png` | HTTP 200, array response, and `userId = 1` |

### Postman Collection Execution Evidence

The following screenshots document the execution of the Postman collection and its test results.

- `evidence/postman/01-postman-run-results-1.png`
- `evidence/postman/02-postman-run-results-2.png`
- `evidence/postman/03-postman-run-results-3.png`

### Tools
- **Charles Proxy:** HTTP/HTTPS traffic inspection.
- **Postman:** Request reproduction and API testing.
- **JavaScript:** Automated assertions using `pm.test`.

### Collection
The exported Postman collection JSON is included in this repository.

### Test API
Requests use [JSONPlaceholder](https://jsonplaceholder.typicode.com/) as a practice API.

**Note:** JSONPlaceholder simulates write operations; changes are not persisted on the server.
