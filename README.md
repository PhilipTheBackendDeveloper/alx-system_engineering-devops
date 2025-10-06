# alx-system_engineering-devops

## 0-simple_web_stack

### Project Overview

This project demonstrates a simple web infrastructure design using a single server hosting a website reachable via the domain **www.foobar.com**.

---

### Infrastructure Components:

- **1 Server** with IP address `8.8.8.8`
- **Web Server:** Nginx
- **Application Server:** Handles application logic and communicates with the web server
- **Application Files:** The codebase of the web application
- **Database:** MySQL for data storage
- **Domain Name:** foobar.com configured with a **www** DNS record pointing to the server IP

---

### Explanation:

1. **What is a server?**  
   A server is a physical or virtual machine that provides services to other devices (clients) over a network.

2. **What is the role of the domain name?**  
   The domain name translates into an IP address via DNS, allowing users to access the website easily without remembering numerical IPs.

3. **What type of DNS record is "www" in www.foobar.com?**  
   It is a **CNAME** (Canonical Name) record that points "www" to the root domain or directly an **A** record pointing to the IP address.

4. **What is the role of the web server?**  
   The web server (Nginx) handles incoming HTTP requests, serves static content, and forwards requests to the application server.

5. **What is the role of the application server?**  
   The application server processes business logic, interacts with the database, and generates dynamic content for the user.

6. **What is the role of the database?**  
   The database (MySQL) stores and manages persistent data required by the application.

7. **What does the server use to communicate with the user's computer?**  
   The server communicates using the **TCP/IP** protocol over the Internet, typically serving HTTP or HTTPS traffic.

---

### Issues with this infrastructure:

- **Single Point of Failure (SPOF):** If the server fails, the website becomes inaccessible.
- **Downtime during maintenance:** Updating or restarting the web server causes temporary unavailability.
- **Limited scalability:** Unable to handle large traffic spikes due to the single server setup.

---

### Diagram

*(You can add a simple diagram here illustrating the server, web server, application server, database, and user flow)*

---

*This completes the simple web stack infrastructure design project.*

