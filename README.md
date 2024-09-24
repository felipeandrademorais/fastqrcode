
# Fast QRcode

Welcome to the Fast QRcode project, an open-source web application designed for generating both static and dynamic QR codes. This project follows clean architecture and clean code principles to ensure scalability and maintainability.

## Project Overview

Fast QRcode allows users to create QR codes that can be static or dynamic. Dynamic QR codes require user authentication and can redirect to user-specified URLs.

### Features

- **Static QR Code Generation:** Generate QR codes instantly without logging in.
- **Dynamic QR Code Generation:** For dynamic QR codes that redirect, user authentication is required.
- **User Dashboard:** Authenticated users can manage their QR codes and modify URLs for dynamic QR codes.

## Technologies Used

- **Frontend:** HTML, CSS, JavaScript (jQuery)
- **Backend:** Node.js with Fastify framework
- **Authentication:** Clerk
- **API:** RESTful API using Node.js (Fastify)

## Project Structure

### Frontend

- `src/`: Contains all source files for the frontend.
  - `js/`: JavaScript files.
  - `css/`: Style sheets.
  - `index.html`: Entry point.
- `dist/`: Built and minified files ready for production.

### Backend

- `src/`: Source files for the backend.
  - `controllers/`: Business logic implementation.
  - `services/`: Service layer handling the business requirements.
  - `models/`: Data models.
- `config/`: Configuration files.
- `tests/`: Test cases for the backend.

## REST API Overview

A REST API is a web service implemented using HTTP and the principles of RESTful architecture. This project's API allows clients to perform CRUD operations on QR codes through HTTP methods like GET, POST, PUT, and DELETE.

### Using jQuery for API Requests

```javascript
// Example: GET request
$.ajax({
  url: 'api/url',
  type: 'GET',
  success: function(result) {
    console.log(result);
  }
});

// Example: POST request
$.ajax({
  url: 'api/url',
  type: 'POST',
  data: { key: 'value' },
  success: function(result) {
    console.log(result);
  }
});
```

## Development Methodology

This project uses the Scrum agile development methodology, which involves sprints, daily stand-ups, and sprint reviews to ensure rapid and flexible response to changes.

## Contributing

Please read CONTRIBUTING.md for details on our code of conduct and the process for submitting pull requests to us.

## Security

HTTP communications are secured and dynamic QR code generation requires user authentication.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
