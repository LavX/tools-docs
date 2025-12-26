# CURL to Code Converter

Convert curl commands to code in multiple programming languages instantly. Perfect for developers, API testing, and documentation.

## Features

- **10+ Programming Languages**: Convert to JavaScript (fetch, axios), Python, Go, Java, PHP, Ruby, Rust, and C#
- **Instant Conversion**: Parse and convert curl commands in milliseconds
- **Full curl Support**: Handles headers, data, authentication, and common curl options
- **Client-Side Processing**: All conversion happens in your browser - no server required
- **Copy to Clipboard**: One-click copy for generated code

## Supported Languages

| Language | Library/Framework | Description |
|-----------|------------------|-------------|
| JavaScript (fetch) | Native browser API | Standard browser fetch API |
| JavaScript (axios) | axios | Popular HTTP client library |
| Python (http.client) | Standard library | Built-in HTTP client |
| Python (requests) | requests | Popular third-party library |
| Go (net/http) | Standard library | Built-in HTTP package |
| Java (HttpURLConnection) | Standard library | Built-in HTTP client |
| PHP (cURL) | cURL extension | PHP cURL wrapper |
| Ruby (Net::HTTP) | Standard library | Built-in HTTP client |
| Rust (reqwest) | reqwest crate | Popular HTTP client |
| C# (HttpClient) | .NET Standard | Built-in HTTP client |

## How to Use

1. **Enter curl command**: Paste your curl command in the input area
2. **Click Convert**: Click the "Convert to Code" button
3. **Select Language**: Choose your target programming language from the available options
4. **Copy Code**: Click "Copy Code" to copy the generated code to your clipboard

## Supported curl Options

The converter supports the following curl options:

- **HTTP Methods**: GET, POST, PUT, DELETE, PATCH, HEAD, OPTIONS
- **Headers**: `-H` or `--header` for custom headers
- **Request Body**: `-d`, `--data`, or `--data-binary` for POST/PUT data
- **Authentication**: Bearer tokens, Basic auth, Digest auth via Authorization header
- **Compression**: `--compressed` flag
- **SSL Options**: `-k` or `--insecure` flag
- **Redirects**: `-L` or `--location` flag
- **Timeout**: `--connect-timeout` or `--max-time`

## Example

### Input curl command:
```bash
curl -X POST https://api.example.com/users \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer token123" \
  -d '{"name":"John Doe","email":"john@example.com"}'
```

### Generated JavaScript (fetch):
```javascript
fetch('https://api.example.com/users', {
  method: 'POST',
  headers: {
    'Content-Type': 'application/json',
    'Authorization': 'Bearer token123',
  },
  body: JSON.stringify({"name":"John Doe","email":"john@example.com"}),
})
  .then(response => response.json())
  .then(data => console.log(data))
  .catch(error => console.error('Error:', error));
```

### Generated Python (requests):
```python
import requests

url = 'https://api.example.com/users'
headers = {
    'Content-Type': 'application/json',
    'Authorization': 'Bearer token123',
}

data = {"name":"John Doe","email":"john@example.com"}
response = requests.post(url, headers=headers, json=data)
print(response.json())
```

## Use Cases

- **API Documentation**: Convert curl examples from API docs to your preferred language
- **Code Generation**: Quickly generate HTTP request code for your projects
- **Testing**: Convert curl commands for testing APIs in different languages
- **Learning**: Understand how to make HTTP requests in different programming languages
- **Migration**: Migrate code from one language to another

## Technical Details

- **Parsing**: Client-side curl command parsing using regex
- **Code Generation**: Template-based code generation for each language
- **Privacy**: All processing happens in your browser - no data is sent to any server
- **Performance**: Instant conversion with no network latency

## Tips

1. **Use quotes**: Always quote URLs and header values in your curl command
2. **JSON data**: For JSON payloads, the converter automatically sets Content-Type header
3. **Authentication**: Include your auth token in the Authorization header
4. **Complex requests**: For complex curl commands, break them down into simpler parts

## Limitations

- Only supports common curl options (see supported options above)
- Does not support multipart file uploads
- Does not support cookies or cookie jars
- Does not support proxy settings
- Does not support all curl flags (focuses on HTTP request essentials)

## Privacy & Security

- All conversion happens client-side in your browser
- No data is sent to any server
- Your curl commands and generated code never leave your device
