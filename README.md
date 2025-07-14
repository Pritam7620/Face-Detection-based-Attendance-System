# Face-Detection-based-Attendance-System
Face Detection Attendance System using Java Spring Boot and OpenCV. Admin and Employees can register and mark attendance via face scan. Attendance is saved in MySQL.


---

## 🛠 Technologies Used
- **Backend**: Java, Spring Boot, Hibernate
- **Frontend**: HTML, CSS, Bootstrap
- **Database**: MySQL
- **Face Detection**: OpenCV (JavaCV)

---

## 👤 Features

### Employee:
- Register with name and face
- Login using ID and role
- Mark Entry and Exit via webcam face scan
- View personal attendance history

### Admin:
- Add new employees
- View all attendance records
- Filter attendance by date
- Manage employee records

---

## ⚙️ How to Run the Project

### 1. Clone or Download
Unzip the folder `Face Detection-based Attendance System.zip` or clone from GitHub.

### 2. Database Setup (MySQL)
- Create a database named `facedetection`
- Import these two files:
  - `facedetection_empface.sql`
  - `facedetection_attendancetbl.sql`

### 3. Configure `application.properties`
Located at `src/main/resources/application.properties`:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/facedetection
spring.datasource.username=root
spring.datasource.password=1972
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
spring.web.resources.static-locations=classpath:/static/,file:faces/
server.port=8080
