Task 2 step 2

<img width="722" height="143" alt="image" src="https://github.com/user-attachments/assets/2f83ff58-fb9e-478c-9b06-57f7d4123dc3" />

This command was executed to see if the cloud project was correctly configured 


Task 2 step 3

<img width="634" height="131" alt="image" src="https://github.com/user-attachments/assets/5c00498a-f764-4133-b989-243b7216d090" />

This command was used to check if a default compute zone was configured. The zone was not configured, so I  set it to us-east1-b 


Task 2 step 4 

<img width="704" height="54" alt="image" src="https://github.com/user-attachments/assets/30031c22-1ecd-4e40-8752-42684429ac90" />

This command was used to set my zone to us-east1-b 

Task 2 Step 5 

<img width="1162" height="281" alt="image" src="https://github.com/user-attachments/assets/c1ca171f-59d6-40d4-89e3-73885b41d42c" />

This command created the Kubernetes cluster 

<img width="671" height="156" alt="image" src="https://github.com/user-attachments/assets/9dc3f8ce-d11d-459b-a50f-01cbc1d285ff" />

This command verifies that the GKE clusters are working as intended 

Task 2 Step 6 

<img width="962" height="77" alt="image" src="https://github.com/user-attachments/assets/3bcb30c7-c956-4bd2-855d-7a7480f57fa8" />

This command configures kubectl and gives it access to the Kubernetes cluster 

Task 2 Step 7 

<img width="781" height="99" alt="image" src="https://github.com/user-attachments/assets/e396528b-e8c6-421e-b27a-d4a855c00416" />

This command verifies that the cluster is connected and shows the worker nodes in the ready state 


Task 3 Step 0 

<img width="1887" height="271" alt="image" src="https://github.com/user-attachments/assets/63fb5a16-8a31-40b6-b4fb-cce8a746b73a" />

This command authenticates my credentials in the terminal


Task 3 step 1

<img width="856" height="68" alt="image" src="https://github.com/user-attachments/assets/4edfe55b-3410-47dc-8e0f-7ac3d2670a60" />

Creates nginx pod 

Task 3 step 2 

<img width="706" height="52" alt="image" src="https://github.com/user-attachments/assets/b87e9622-8d20-474e-af9b-cdcbaeb8ebb7" />

Creates a server pod that will act as a backend web server 

Task 3 step 3 

<img width="703" height="49" alt="image" src="https://github.com/user-attachments/assets/ee31149e-4712-475d-9026-ab7087d29f02" />

Creates a client pod that will act as a client and send HTTP requests 


Task 3 step 4 

<img width="931" height="120" alt="image" src="https://github.com/user-attachments/assets/8dc48612-0487-42ad-93fe-0960040ea6f3" />

Verifies that the pods are all running 


Task 3 step 5 

<img width="849" height="73" alt="image" src="https://github.com/user-attachments/assets/7b11ff4e-db8c-4362-8be2-62f4c9586f8c" />

This command displays all worker nodes 


Task 3 step 6 

<img width="975" height="422" alt="image" src="https://github.com/user-attachments/assets/4220dfe8-de3f-43c7-aed4-e96b0938571f" />

This command uses localhost to test the pod locally 


Task 3 step 7 

<img width="830" height="85" alt="image" src="https://github.com/user-attachments/assets/f4bedcff-e7d8-4e5f-9c6b-6e204d618ba0" />

This command retrieves the server IP address 

Task 3 step 8 


<img width="1080" height="424" alt="image" src="https://github.com/user-attachments/assets/32b14be4-5aef-44ac-81b9-4492cf667b22" />

This command accesses the server using the IP we just retrieved 

Task 4 step 1 

<img width="802" height="103" alt="image" src="https://github.com/user-attachments/assets/f4aae210-97a0-41ed-b3c3-8626f91a8bf0" />

Creates a service for the server pod named server service 


Task 4 step 2 


<img width="817" height="78" alt="image" src="https://github.com/user-attachments/assets/454cdce6-bb6e-4e82-a4c6-c38c007fb872" />

Verifies/Displays the service 

Task 4 step 3 

<img width="1027" height="332" alt="image" src="https://github.com/user-attachments/assets/3ed73b37-518b-43db-ad94-31fdd0915ce1" />

This command is used to inspect service details 




Task 4 step 4 

<img width="880" height="92" alt="image" src="https://github.com/user-attachments/assets/04fc527a-a21a-4389-a706-e9574cb3cd98" />

This command creates a temporary debug pod that helps verify the qualified DNS name 

Task 5 step 1 

<img width="1067" height="390" alt="image" src="https://github.com/user-attachments/assets/c61b711d-e13f-4035-b404-0fa0681a465d" />

This command finds the DNS name and ClusterIP

Task 6 Step 1 

<img width="822" height="426" alt="image" src="https://github.com/user-attachments/assets/a662431b-caec-435b-b523-b1154203c982" />

Send traffic to the service pod from the client pod 

Task 6 step 2 

<img width="823" height="432" alt="image" src="https://github.com/user-attachments/assets/816558d5-4ef9-4f53-aa0a-4ec651ea114e" />

The same command as the previous step is run multiple times to send traffic 


Task 7 step 1 
<img width="941" height="270" alt="image" src="https://github.com/user-attachments/assets/e85749c6-4801-48b1-89a8-382c4b02135a" />



Clean up to avoid charges 



Reflection Questions 

1. The management of an application using only Docker would rely heavily on manual Docker commands. The user would need to manually configure ports, environment variables, and container networking. As the number of containers increases, several challenges arise, including manual scaling and ongoing maintenance of containers. If a container crashes, it must be restarted manually, since Docker alone does not provide automatic recovery or self-healing. This approach becomes increasingly difficult to manage as the application grows in size and complexity.


2. A Pod is the smallest unit that can be deployed and managed in Kubernetes. Kubernetes treats Pods as the smallest unit because they allow related containers to be grouped together and managed as a single cohesive unit rather than individually. Containers are too low-level to be managed directly at scale, so Pods act as a bridge that provides shared networking, storage, and lifecycle management. This abstraction makes applications easier to deploy, scale, and maintain.

3. Services are needed in Kubernetes because Pods are temporary and their IP addresses can change, which means connections would constantly break. A Service provides stability by offering a consistent network endpoint that routes traffic to the correct Pods, even as Pods are created, destroyed, or replaced. This allows applications and microservices to communicate reliably without depending on changing Pod IP addresses.

4. DNS-based service discovery in Kubernetes automatically creates DNS records for each Service. This allows Pods to use a Service’s DNS name to communicate with it instead of relying on Pod IP addresses. Because Pod IPs can change, using DNS ensures stable and reliable communication. Service discovery is considered a core requirement for Microservices Architecture because microservices are designed to be loosely coupled, independently deployed, and dynamically scaled. In such an environment, service instances are constantly changing, making hard-coding network locations impractical.

5.Applications should be run through multiple containerized services managed by Kubernetes. Kubernetes allows applications to scale easily by running multiple replicas of individual services instead of scaling the entire system at once. This makes better use of resources and supports growing workloads. In a single-machine system, a failure can take down the entire application, while Kubernetes isolates failures to individual services or Pods. 

Diagram

<img width="788" height="589" alt="image" src="https://github.com/user-attachments/assets/3c60b018-f750-4a13-be29-0b00bfed3d63" />



