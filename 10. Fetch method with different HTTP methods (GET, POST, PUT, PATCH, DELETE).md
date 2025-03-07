| **HTTP Method** | **Description** | **Syntax** | **Example** |
|-----------------|-----------------|-----------|-------------|
| **GET** | Fetches data from the server. | `fetch(url)` | ```fetch('https://api.example.com/data')<br>.then(response => response.json())<br>.then(data => console.log(data))<br>.catch(error => console.error('Error:', error));``` |
| **POST** | Sends data to the server (usually to create a new resource). | `fetch(url, { method: 'POST', headers: { 'Content-Type': 'application/json' }, body: JSON.stringify(data) })` | ```fetch('https://api.example.com/data', {<br>  method: 'POST',<br>  headers: { 'Content-Type': 'application/json' },<br>  body: JSON.stringify({ name: 'John', age: 30 })<br>})<br>.then(response => response.json())<br>.then(data => console.log('Created:', data))<br>.catch(error => console.error('Error:', error));``` |
| **PUT** | Updates or replaces a resource on the server. | `fetch(url, { method: 'PUT', headers: { 'Content-Type': 'application/json' }, body: JSON.stringify(data) })` | ```fetch('https://api.example.com/data/1', {<br>  method: 'PUT',<br>  headers: { 'Content-Type': 'application/json' },<br>  body: JSON.stringify({ name: 'Jane', age: 25 })<br>})<br>.then(response => response.json())<br>.then(data => console.log('Updated:', data))<br>.catch(error => console.error('Error:', error));``` |
| **PATCH** | Partially updates a resource on the server. | `fetch(url, { method: 'PATCH', headers: { 'Content-Type': 'application/json' }, body: JSON.stringify(data) })` | ```fetch('https://api.example.com/data/1', {<br>  method: 'PATCH',<br>  headers: { 'Content-Type': 'application/json' },<br>  body: JSON.stringify({ age: 26 })<br>})<br>.then(response => response.json())<br>.then(data => console.log('Partially updated:', data))<br>.catch(error => console.error('Error:', error));``` |
| **DELETE** | Deletes a resource on the server. | `fetch(url, { method: 'DELETE' })` | ```fetch('https://api.example.com/data/1', {<br>  method: 'DELETE'<br>})<br>.then(response => {<br>  if (response.ok) {<br>    console.log('Deleted successfully');<br>  } else {<br>    console.error('Error deleting data');<br>  }<br>})<br>.catch(error => console.error('Error:', error));``` |

### Notes:
- `url`: The endpoint to which the request is made.
- `method`: The HTTP method (`GET`, `POST`, `PUT`, `PATCH`, `DELETE`).
- `headers`: Defines the content type (e.g., `application/json` for JSON data).
- `body`: The payload of the request, typically used for `POST`, `PUT`, and `PATCH`.
