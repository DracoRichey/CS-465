# CS-465
Travlr Getaways – Full Stack Web Application
Architecture

This project uses two different frontend approaches to support different user needs. The customer-facing side of the application was built using Express, HTML, CSS, JavaScript, and Handlebars templates. This approach follows a traditional server-rendered Model–View–Controller (MVC) architecture, where pages are generated on the server and sent to the browser. It is well suited for public-facing content where users primarily browse and view travel information.

The administrative side of the application was built as a Single Page Application (SPA) using Angular. The Angular SPA runs entirely in the browser and communicates with the backend through RESTful API calls. Unlike the Express frontend, the SPA does not require full page reloads when data changes, which provides a more responsive and efficient user experience for administrative tasks such as adding and managing travel packages.

The backend uses a NoSQL MongoDB database because it provides flexibility in data modeling and integrates naturally with JavaScript-based technologies like Node.js and Express. MongoDB’s document-based structure allows travel package data to be stored and retrieved efficiently without rigid table schemas, which supports scalability and rapid development.

Functionality

JSON differs from JavaScript in that it is a lightweight data-interchange format, not a programming language. While JavaScript contains logic, functions, and execution flow, JSON is strictly used to structure and transmit data. In this project, JSON is the primary format used to exchange data between the frontend and backend, allowing Angular and Express to communicate consistently through API requests and responses.

Throughout development, code was refactored to improve functionality and efficiency. Static HTML pages were converted into Handlebars templates to enable dynamic rendering of trip data. On the administrative side, Angular components were reused to handle similar UI tasks, such as displaying trip lists and submitting form data. Reusable UI components reduce duplication, improve maintainability, and make it easier to update or extend the application without rewriting large portions of code.

Testing

The application was tested using multiple API testing methods to verify correct request handling and data retrieval. HTTP methods such as GET and POST were used to retrieve travel data and create new travel packages. Endpoints were tested both through the Angular SPA and directly using Postman to confirm proper API behavior.

Additional testing complexity was introduced with the addition of security. Administrative endpoints were secured using JSON Web Tokens (JWT), requiring authentication for protected operations. Postman was used to verify that unauthorized requests were rejected and that authenticated requests with valid tokens were allowed. This testing confirmed that endpoint security, request methods, and data validation were functioning correctly within the full stack application.

Reflection

This course significantly advanced my understanding of full stack web development and how frontend and backend components work together in a real-world application. I gained hands-on experience with Express, Angular, MongoDB, RESTful APIs, and authentication using JWTs. These skills strengthened my ability to design application architecture, integrate databases, and implement secure administrative functionality.

Completing this project helped me become more confident working with modern web development frameworks and tools. The experience of building, testing, securing, and documenting a full stack application has made me a more marketable candidate by demonstrating practical skills that are directly applicable to entry-level software development roles.
