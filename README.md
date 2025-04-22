# CS-305-Portfolio

### Who was the client? What did they need?
The client was **Artemis Financial**, a company that provides personalized financial planning. They wanted to enhance the security of their application by verifying transferred data using a checksum and ensuring encrypted communication over HTTPS.

### What did you do well when finding security vulnerabilities?
I identified and addressed potential vulnerabilities by:
- Implementing **SHA-256 hashing** for checksum validation
- Configuring the application for **HTTPS** using a self-signed SSL certificate
- Using **OWASP Dependency-Check** to scan for vulnerable libraries

These efforts are essential for protecting sensitive data and maintaining client trust in a financial application.

### Which part was challenging or helpful?
Setting up and troubleshooting the **HTTPS configuration** with `keystore.p12` was initially challenging due to certificate path issues and self-signed certificate browser warnings. However, successfully securing the route was rewarding and educational.

### How did you increase layers of security?
I added:
- A SHA-256 checksum endpoint
- HTTPS encryption using Java Keytool
- Static vulnerability testing with OWASP Dependency-Check

In future projects, I would continue using OWASP tools and add **dynamic analysis** or **penetration testing** for deeper assessments.

### How did you ensure the code was functional and secure?
After refactoring the code, I:
- Ran `mvn clean install` to verify build success
- Confirmed the `/hash` route responded securely over HTTPS
- Reviewed the **dependency-check HTML report** to ensure no new vulnerabilities were introduced

### Tools and practices used:
- **Java SHA-256** implementation
- **Spring Boot SSL configuration**
- **Java Keytool**
- **OWASP Dependency-Check Maven plugin**
- **Functional testing** in browser and terminal

### What can I show future employers?
This project showcases my ability to:
- Implement encryption and hashing
- Configure SSL/TLS in Spring Boot
- Perform secure code reviews and vulnerability scans
- Follow software security best practices from end to end
