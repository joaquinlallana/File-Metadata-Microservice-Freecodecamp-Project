# File Metadata Microservice

A simple microservice that analyzes uploaded files and returns their metadata (name, type, and size in bytes). Built as part of the [FreeCodeCamp Back End Development and APIs Certification](https://www.freecodecamp.org/learn/back-end-development-and-apis/).

## 🚀 Features
- Accepts file uploads via a web form or API endpoint.
- Returns JSON response with:
  - `name`: Original filename.
  - `type`: MIME type (e.g., `image/png`).
  - `size`: File size in bytes.

## ⚙️ How It Works
1. **Frontend**: User uploads a file through the HTML form.
2. **Backend**: The server processes the file using `multer` middleware.
3. **Response**: Returns metadata as JSON (e.g., `{"name":"example.txt","type":"text/plain","size":123}`).

## 📦 Installation
1. Clone the repo:
   ```bash
   git clone https://github.com/joaquinlallana/File-Metadata-Microservice-Freecodecamp-Project.git
   ```
2. Install dependencies:

```bash

npm install
```
3. Start the server:

```bash

    npm start

    Open http://localhost:3000 in your browser.
```

# 🌐 API Reference

## Upload a file

    Endpoint: POST /api/fileanalyse

    Request:

        Form field name: upfile (must be a file upload).

    Response:
    ```json

    {
      "name": "filename.ext",
      "type": "file/mimetype",
      "size": 1234
    }
    ```

# 🧪 Testing

Run the included functional tests (FreeCodeCamp requirements) with:
```bash

npm test
   ```
# 📝 Notes

    Max file size: Limited by multer (adjust in server.js if needed).

    Supported files: Any MIME type (e.g., images, text, PDFs).

# 🔧 Dependencies

    Express.js

    Multer (for file handling)

    Mocha/Chai (for testing)

# 🙌 Credits

Project idea by FreeCodeCamp.
Developed by Joaquín Lallana.