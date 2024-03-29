# Job Lens
Microservices driven platform for companies to post their job listings and employees to leave reviews for companies they have worked for

## Tech Stack 
Developed using:
Java, Spring Boot, Spring Data JPA, PostgreSQL, Spring Cloud Gateway, Spring Cloud Netflix - Eureka Server, Zipkin, Spring Cloud OpenFeign, Micrometer

## Services Involved
* [API Gateway](https://github.com/SinghVikram97/api-gateway): Serves as the single entrypoint for the client and routes request to different services
* [Eureka Server](https://github.com/SinghVikram97/service-registry): Provides service registry and load balancing capabilities
* [Company Microservice](https://github.com/SinghVikram97/company-service): Manages the creation, modification, and retrieval of Company related data
* [Job Microservice](https://github.com/SinghVikram97/job-service): Manages the creation, modification, and retrieval of Jobs related data
* [Review Microservice](https://github.com/SinghVikram97/review-service): Manages the creation, modification, and retrieval of Reviews related data

## High Level Design
![Job Lens Zoomed](https://github.com/SinghVikram97/Job-Lens/assets/18444000/07a3454b-5d7c-4cb0-9ecd-c16120e97630)

## LLD
### Company Service
* Create Company POST (/api/companies)
<img width="510" alt="image" src="https://github.com/SinghVikram97/Job-Lens/assets/18444000/3d270826-c2d3-4462-8b06-43ceee093539">

* Update Company PUT (/api/companies/{companyId})
![Seq](https://github.com/SinghVikram97/Job-Lens/assets/18444000/a40ff51d-adc7-4443-a568-c2f5c025f3e6)

* Get Company GET (/api/companies/{companyId})
![Seq](https://github.com/SinghVikram97/Job-Lens/assets/18444000/0bdfb3ed-6633-4642-b676-90f963234f9d)

* Delete Company DELETE (/api/companies/{companyId})
![Seq](https://github.com/SinghVikram97/Job-Lens/assets/18444000/b4a6ba08-2d9a-4fe8-8482-2d3cce9dade4)

