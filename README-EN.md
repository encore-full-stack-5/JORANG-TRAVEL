# ✈️ Everything About JORANG Travel

## <br>📃 Project Development Motivation
We developed this service to check how others think about and plan their trips to destinations I want to visit, based on our common interest in overseas travel.<br><br>

## 📃 Project Goals
Let’s write what I use correctly.<br><br>

## 📃 Project Introduction
I can manage my travel journal and actual expenses, share them with others, and gain information needed to prepare for my trip by reading and interacting with other people's travel experiences.<br><br>

## 📃 Project Duration
2024/6/3 ~ 2024/7/1<br><br>

## 📃 Core Features
### 1. Writing and Sharing Travel Journals, Expenses, and Plans

- Writing and sharing travel journals and expenses by date
- Uploading and retrieving photos using Google Cloud Storage
- Implementing an image slider
- Visualizing expenses in charts
- Implementing sorting of travel journals by recency and likes, as well as filtering by travel duration
- Sending a temporary password via email when user ID or email is changed<br><br>

### 2. Chatbot (See Chatbot server below)

- Implementing features to recommend attractions, destinations, travel plans, and personalized travel plan suggestions using Langchain 
  (LLM: Google Gemini)<br><br>

### Main Server (Java with Spring Boot)
https://github.com/encore-full-stack-5/JORANG-TRAVEL-BE

### Chatbot Server (Python with FastAPI, Langchain)
https://github.com/encore-full-stack-5/JORANG_LANGCHAIN_SERVER

### Front End (React)
https://github.com/encore-full-stack-5/JORANG-TRAVEL-FE<br><br>

## 🧑🏻‍💻 Team Members and Roles
 
 - Jinho Jo: Writing travel journals by date, uploading and retrieving photos, user authentication (JWT), web security, search functionality, overall debugging
 - Sehyun Kim: Publishing, user login, registration, email sending, implementing country introduction features 
 - Seoyeon Lim : Implementing the function to write travel expenses by date
 - Common: Implementing chatbot features (recommendations for attractions, destinations, travel plans, and personalized travel plans)<br><br>

## 📃 Screen Configuration and Feature Introduction (Video)
### 1. Checking Travel Journals by Country ###

https://github.com/user-attachments/assets/a2ea9a2e-9f42-490c-aff8-9575c6e234fd

### <br> 2. Checking All Travel Journals ###

https://github.com/user-attachments/assets/b5763e68-649d-4c56-b9f9-6a492f1f1b8f

### <br> 3. Writing and Sharing Travel Journals ###

https://github.com/user-attachments/assets/a62dcd25-fe13-4b7b-92ee-a55645de2555

### <br> 4. Temporarily Saving and Modifying Travel Journals ###

https://github.com/user-attachments/assets/bb1a542d-729c-4390-8eb5-7b50abc26043

### <br> 5. Travel Chatbot ###

https://github.com/user-attachments/assets/5277301b-6221-4451-9c30-7a4ac4897c13

## <br> ⚙️ Tech Stack

### Server Language and Framework
![Java](https://img.shields.io/badge/java-%23ED8B00?style=for-the-badge&logoColor=white)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Spring-Boot](https://img.shields.io/badge/spring--boot-%236DB33F.svg?style=for-the-badge&logo=springboot&logoColor=white)
![FASTAPI](https://img.shields.io/badge/FASTAPI-%23009688?style=for-the-badge&logo=fastapi&logoColor=white)

### Database
<img src="https://img.shields.io/badge/mysql-4479A1?style=for-the-badge&logo=mysql&logoColor=white">

### Image storage
![Google Cloud Storage](https://img.shields.io/badge/google%20cloud%20storage-%23AECBFA?style=for-the-badge&logo=googlecloudstorage&logoColor=black)

### LLM
![Google gemini](https://img.shields.io/badge/google%20gemini-%238E75B2?style=for-the-badge&logo=googlegemini&logoColor=white)

### Frontend
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)<br><br>

   
## Reflections
### Jinho 
Overall, this project allowed me to experience the entire process from front to back, which greatly contributed to my growth. During this process, I encountered many errors and was able to broaden my perspective on various error cases. In particular, I gained deep insights into how to query based on join relationships. Through this, I personally felt why N+1 loading occurs and how to solve it with fetch join. Additionally, as a team leader, I often had to read other people's code, which helped me develop an understanding of others' code and realize parts I had overlooked. Through this process, I felt that reading not only my code but also other people's code is very helpful for skill improvement. A point of regret was that I was unable to implement the elastic search setup due to time-consuming certificate issues. Also, to automatically delete child entities when deleting a parent entity, I used cascade with bidirectional mapping. However, this led to circular references, and to avoid this, I used @JsonManagedReference and @JsonBackReference, but ultimately, the data size of the parent entity became too large. I realized that replacing data deletion with an isDeleted flag and avoiding circular references by using DTOs would be a better approach. I also aimed to resolve everything with JPA named queries, but I faced the limitation of JPQL, which cannot handle joins of three tables and LIMIT. This made me realize the necessity of using native SQL queries to fetch only the required data at once instead of relying too much on ORM. Lastly, while debugging, I realized more problems than expected, and by solving them, I understood the importance of the configuration of buttons and the convenience of the server API.<br>
<br>
### Sehyun
While working on the JORANG project, I was able to overcome various difficulties and learn a lot. At first, it was challenging to see multiple errors and fix them, but after experiencing recurring errors a few times, I became capable of fixing them myself. I regret not being able to utilize Redis during the initial design and modification of the ERD, and I hope to use it in the next project. While implementing the chatbot page, connecting a different Python server to Spring Boot initially felt complicated, but I realized it was simpler than expected once I connected the servers. I learned how to use Langchain, but I regret not being able to utilize it fully due to time constraints. I also learned how to use Axios to send and receive data between the front end and the server, which helped me understand the basics of data communication. Initially, I struggled with asynchronous functions due to lack of knowledge, but while working on the project, I studied async and await and gained an understanding of asynchronous functions. Although I found it confusing to structure the front end components at first, I was able to understand the overall flow, structure, and functionality of React in greater detail by building the screen from scratch. Additionally, there was an issue with class name conflicts when using CSS, but I managed to prevent collisions by carefully managing class names and establishing naming conventions. I also encountered a problem where the screen did not render as expected in React, but after studying the rendering criteria and useEffect in detail, I was able to understand React's rendering mechanism and construct the screen as desired. This project provided me with valuable experiences in overcoming various technical difficulties in both the back end and front end.<br>
<br>
### Seoyeon
By implementing the request and response process through the API, I learned how the server reacts to the client's requests and provides the necessary data. I experienced a problem where the code became excessively lengthy due to not clearly separating components in the front component structure, which reduced overall code readability. This made it difficult to find information within the code and decreased maintenance efficiency. There were also issues with class name conflicts in CSS. I realized that I need to pay more attention to component design in the future.
