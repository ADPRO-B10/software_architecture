# B10 software_architecture
**C4 Model:** https://drive.google.com/file/d/1iPoVWhCQ7GrsJKCGQAS8KCda2GTB0GEM/view?usp=sharing
## 1. The current architecture of group …. , the context, container and deployment diagram

### Context Diagram
![CONTEXT DIAGRAM](https://github.com/ADPRO-B10/software_architecture/assets/112263712/a1dc0349-8670-4d4e-8efe-81563b7fb91d)

![alt text](current.png)

## 2. The future architecture of group …
![FUTURE ARCHITECTURE (1)](https://github.com/ADPRO-B10/software_architecture/assets/112263712/fa11d842-7680-455f-b501-f31b649277e8)

## 3. Explanation of risk storming of group …

1. **DNS (Domain Name System)**: Routes user requests to the appropriate load balancer.
   **Risks:**
   - DNS Spoofing/Cache Poisoning: Hackers might manipulate DNS entries, redirecting users to malicious sites.
   - DDoS (Distributed Denial of Service) Attacks: attacks targeting DNS servers can disrupt the service.
     
3. **Load Balancer:** Distributes incoming traffic across multiple frontend virtual machines (VMs) to ensure high availability and reliability.
  **Single Point of Failure:** If the load balancer fails, the entire service can become unavailable.
  **Misconfiguration:** Incorrect settings can lead to inefficient traffic distribution.

5. **Frontend Microservice:** Runs on VMs that handle user interfaces and user interactions.
6. **Backend Microservices:** Each backend service runs on its own VM and handles specific business logic or data processing tasks.

## 4. Microservices Diagram
## Shopping Cart Component
![SHOPPING CART COMPONENT](https://github.com/ADPRO-B10/software_architecture/assets/112263712/94621919-691a-42d5-ab75-81f66eab82d7)

