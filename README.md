[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/m9BZqBrx)
**<ins>Note</ins>: Students must update this `README.md` file to be an installation manual or a README file for their own CS403 projects.**

**รหัสโครงงาน:** 67-2_01_tpb-r2

**ชื่อโครงงาน (ไทย):** การออกแบบและพัฒนาเว็บแอปพลิเคชันระบบค้นหาและแสดงโครงงานพิเศษของสาขาวิทยาการคอมพิวเตอร์ มหาวิทยาลัยธรรมศาสตร์ 

**Project Title (Eng):** WEB APPLICATION FOR SEARCHING ABD DISPLAYING SPECIAL PROJECTS OF THE COMPUTER SCIENCE DEPARTMENT AT THAMMASAT UNICERSITY

**อาจารย์ที่ปรึกษาโครงงาน:** ผศ.ดร.ฐาปนา บุญชู 

**ผู้จัดทำโครงงาน:** (โปรดเขียนข้อมูลผู้จัดทำโครงงานตามฟอร์แมตดังแสดงในตัวอย่างด้านล่าง)
1. นางสาวมัสลิน พัสตร์วาณิช  6409682843  muslin.pat@dome.tu.ac.th
2. นายสันติภาพ พิพัฒน์รัตนชัย 6509612047  santipap.pip@dome.tu.ac.th
   

# Directory tree
```text
frontend/
├─ public/
│
├─ src/
│  ├─ api/
│  │  └─ axiosConfig.ts
│  │
│  ├─ assets/
│  │  ├─ background.css
│  │  ├─ logo.png
│  │  └─ react.svg
│  │
│  ├─ components/
│  │  ├─ admin/
│  │  │  ├─ ConfirmDialog.tsx
│  │  │  └─ RoleFilter.tsx
│  │  │
│  │  ├─ project/
│  │  │  ├─ ProjectAbstract.tsx
│  │  │  ├─ ProjectActionButtons.tsx
│  │  │  ├─ ProjectHeader.tsx
│  │  │  ├─ ProjectInfo.tsx
│  │  │  └─ ProjectSection.tsx
│  │  │
│  │  ├─ AccountSideBar.tsx
│  │  ├─ EditProjectForm.tsx
│  │  ├─ FilterDropMenu.tsx
│  │  ├─ FilterMultiChoice.tsx
│  │  ├─ FilterSingleSelect.tsx
│  │  ├─ FooterKeywords.tsx
│  │  ├─ HistorySorting.tsx
│  │  ├─ MyProjectCard.tsx
│  │  ├─ NavBar.tsx
│  │  ├─ Pagination.tsx
│  │  ├─ ProjectCard.tsx
│  │  ├─ ProjectForm.tsx
│  │  ├─ SideBar.tsx
│  │  ├─ Sorting.tsx
│  │  └─ TextSearch.tsx
│  │
│  ├─ context/
│  │  └─ AuthContext.tsx
│  │
│  ├─ dto/
│  │  └─ ProjectDTO.ts
│  │
│  ├─ pages/
│  │  ├─ admin/
│  │  │  ├─ AdminPanel.tsx
│  │  │  ├─ ApprovedUsers.tsx
│  │  │  ├─ DownloadHistoryList.tsx
│  │  │  ├─ PendingUsers.tsx
│  │  │  └─ ProjectList.tsx
│  │  │
│  │  ├─ AboutCSTU.tsx
│  │  ├─ AddProject.tsx
│  │  ├─ Browse.tsx
│  │  ├─ ChangePassword.tsx
│  │  ├─ EditProject.tsx
│  │  ├─ Favorite.tsx
│  │  ├─ ForgotPassword.tsx
│  │  ├─ Guest.tsx
│  │  ├─ GuestRegister.tsx
│  │  ├─ History.tsx
│  │  ├─ Home.tsx
│  │  ├─ Login.tsx
│  │  ├─ Overview.tsx
│  │  ├─ PendingApproval.tsx
│  │  ├─ Project.tsx
│  │  ├─ Student.tsx
│  │  └─ TULogin.tsx
│  │
│  ├─ route/
│  │  ├─ AppRoutes.tsx
│  │  └─ ProtectedRoute.tsx
│  │
│  ├─ App.css
│  ├─ App.tsx
│  ├─ index.css
│  ├─ main.tsx
│  └─ vite-env.d.ts
│
├─ eslint.config.js
├─ index.html
├─ package.json
├─ package-lock.json
├─ README.md
├─ tailwind.config.js
├─ tsconfig.json
├─ tsconfig.app.json
├─ tsconfig.node.json
└─ vite.config.ts


├─ backend/
│  ├─ .mvn/                          # Maven wrapper
│  ├─ src/
|  │  ├─ main/
|  │  │  ├─ java/th/ac/tu/cs/projectportal/
|  │  │  │   ├─ config/
│  │  │  │   │  ├─ AdminSeeder.java
│  │  │  │   │  ├─ CorsConfig.java
│  │  │  │   │  ├─ ProjectConfig.java
│  │  │  │   │  └─ SecurityConfig.java
│  │  │  │   │
│  │  │  │   ├─ controller/
│  │  │  │   │  ├─ AdminController.java
│  │  │  │   │  ├─ BookmarkController.java
│  │  │  │   │  ├─ DownloadHistoryController.java
│  │  │  │   │  ├─ HistoryController.java
│  │  │  │   │  ├─ ProjectController.java
│  │  │  │   │  ├─ PublicDownloadHistoryController.java
│  │  │  │   │  ├─ PublicProjectController.java
│  │  │  │   │  └─ UserController.java
│  │  │  │   │
│  │  │  │   ├─ dto/
│  │  │  │   │  ├─ ProjectDTO.java
│  │  │  │   │  └─ UserResponseDTO.java
│  │  │  │   │
│  │  │  │   ├─ entity/
│  │  │  │   │  ├─ Bookmark.java
│  │  │  │   │  ├─ BookmarkId.java
│  │  │  │   │  ├─ DownloadHistory.java
│  │  │  │   │  ├─ DownloadHistoryId.java
│  │  │  │   │  ├─ Gender.java
│  │  │  │   │  ├─ History.java
│  │  │  │   │  ├─ HistoryId.java
│  │  │  │   │  ├─ Project.java
│  │  │  │   │  ├─ Role.java
│  │  │  │   │  └─ User.java
│  │  │  │   │
│  │  │  │   ├─ repository/
│  │  │  │   │  ├─ BookmarkRepository.java
│  │  │  │   │  ├─ DownloadHistoryRepository.java
│  │  │  │   │  ├─ HistoryRepository.java
│  │  │  │   │  ├─ ProjectRepository.java
│  │  │  │   │  └─ UserRepository.java
│  │  │  │   │
│  │  │  │   ├─ service/
│  │  │  │   │  ├─ DownloadHistoryService.java
│  │  │  │   │  ├─ ProjectService.java
│  │  │  │   │  ├─ UserCleanupService.java
│  │  │  │   │  └─ UserService.java
│  │  │  │   │
│  │  │  │   └─ BackendApplication.java
│  │  │  │
│  │  │  └─ resources/
│  │  │     ├─ sql/
│  │  │     │  └─ schema.sql
│  │  │     ├─ application.properties
│  │  │     └─ application-dev.properties
│  │  │
│  │  └─ test/
│  │     └─ java/th/ac/tu/cs/projectportal/
│  │  │  │  └─ BackendApplicationTests.java
│  │
│  └─ target/                      
│
├─ .gitattributes
├─ mvnw
├─ mvnw.cmd
└─ pom.xml
```

# 🔧 Prerequisites
## 📌 Software ที่ต้องติดตั้งก่อน

#### 1. Git

ใช้สำหรับ clone repository

```bash
git --version
```
---

#### 2. Frontend

* Node.js **LTS (แนะนำ 20.x หรือ 22.x)**
* npm (มากับ Node.js)

ตรวจสอบเวอร์ชัน:

```bash
node -v
npm -v
```

#### 3. Backend

* Java **JDK 25**

ตรวจสอบเวอร์ชัน:

```bash
java -version
javac -version
```

#### 4. Database

* **MySQL Server 8.x**
* **MySQL Workbench** (ใช้สำหรับจัดการฐานข้อมูล)

---

#### 5. Visual Studio Code**
**Extension ที่ควรมี
* **Spring boot extension pack**
* **Extension Pack for Java**


---

# 🚀 Getting Started

### 1️⃣ Clone Repository

```bash
git clone <repository-url>
```
```bash
cd <project-root>
```

---

## 🖥️ Frontend Setup (React + Vite)

### 📂 เข้าโฟลเดอร์ frontend

```bash
cd frontend
```

### 📦 ติดตั้ง dependencies

```bash
npm install
```

> คำสั่งนี้จะติดตั้ง React, Vite, TypeScript, Tailwind, MUI, Axios และ library อื่น ๆ 

### ▶️ รัน Frontend (Development Mode)

```bash
npm run dev
```

เปิดเบราว์เซอร์ที่:

```
http://localhost:5173
```

---

## ⚙️ Backend Setup (Spring Boot)

### 📂 เข้าโฟลเดอร์ backend

```bash
cd backend
```

### ▶️ รัน Backend

#### Windows

```powershell
.\mvnw.cmd spring-boot:run
```

#### macOS / Linux

```bash
./mvnw spring-boot:run
```
#### รัน Spring Boot Application

สามารถรันได้ 2 วิธี:

##### วิธีที่ 1: ผ่าน Spring Boot Dashboard

เปิดแท็บ Spring Boot Dashboard

เลือกชื่อแอปพลิเคชัน

กด ▶️ Run

##### วิธีที่ 2: ผ่านไฟล์หลัก

เปิดไฟล์ 

backend/src/main/java/th/ac/tu/cs/projectportal/BackendApplication.java

กด ▶️ Run ที่อยู่เหนือเมธอด main()

> โปรเจกต์นี้ใช้ **Maven Wrapper** จึงไม่จำเป็นต้องติดตั้ง Maven เอง

Backend จะรันที่:

```
http://localhost:8081
```

---

### 🛢️ Database Configuration

โปรเจกต์นี้ใช้ **MySQL Server** และจัดการฐานข้อมูลผ่าน **MySQL Workbench**

#### ขั้นตอนเตรียมฐานข้อมูล

1. เปิด MySQL Workbench และเชื่อมต่อ MySQL Server
2. สร้าง database ใหม่ (เช่น `finalproject`)
3. ตรวจสอบว่า MySQL Server ทำงานที่ port `3306`

#### ตั้งค่าใน Backend

สร้างไฟล์ `backend/src/main/resources/application-dev.properties`

ตัวอย่าง:

```properties

# Database configuration
db.host=localhost
db.port=3306
db.name=finalproject

spring.datasource.username=root
spring.datasource.password=root

# Backend server port
server.port=8081
```
---
