[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/m9BZqBrx)
**<ins>Note</ins>: Students must update this `README.md` file to be an installation manual or a README file for their own CS403 projects.**

**รหัสโครงงาน:** 67-2_01_tpb-r2

**ชื่อโครงงาน (ไทย):** การออกแบบและพัฒนาเว็บแอปพลิเคชันระบบค้นหาและแสดงโครงงานพิเศษของสาขาวิทยาการคอมพิวเตอร์ มหาวิทยาลัยธรรมศาสตร์ 

**Project Title (Eng):** WEB APPLICATION FOR SEARCHING ABD DISPLAYING SPECIAL PROJECTS OF THE COMPUTER SCIENCE DEPARTMENT AT THAMMASAT UNICERSITY

**อาจารย์ที่ปรึกษาโครงงาน:** ผศ.ดร.ฐาปนา บุญชู 

**ผู้จัดทำโครงงาน:** (โปรดเขียนข้อมูลผู้จัดทำโครงงานตามฟอร์แมตดังแสดงในตัวอย่างด้านล่าง)
1. นางสาวมัสลิน พัสตร์วาณิช  6409682843  muslin.pat@dome.tu.ac.th
2. นายสันติภาพ พิพัฒน์รัตนชัย 6509612047  santipap.pip@dome.tu.ac.th
   
Manual / Instructions for your projects starts here !
# Directory tree
├─ backend/

│  ├─ .mvn/                          # Maven wrapper

│  ├─ src/

|  │  │  ├─ main/

|  │  │  │  ├─ java/th/ac/tu/cs/projectportal/

|  │  │  │  │  |  ├─ config/
│  │  │  │  |  |  |  │  ├─ AdminSeeder.java
│  │  │  │                 │  ├─ CorsConfig.java
│  │  │  │                 │  ├─ ProjectConfig.java
│  │  │  │                 │  └─ SecurityConfig.java
│  │  │  │                 │
│  │  │  │                 ├─ controller/
│  │  │  │                 │  ├─ AdminController.java
│  │  │  │                 │  ├─ BookmarkController.java
│  │  │  │                 │  ├─ DownloadHistoryController.java
│  │  │  │                 │  ├─ HistoryController.java
│  │  │  │                 │  ├─ ProjectController.java
│  │  │  │                 │  ├─ PublicDownloadHistoryController.java
│  │  │  │                 │  ├─ PublicProjectController.java
│  │  │  │                 │  └─ UserController.java
│  │  │  │                 │
│  │  │  │                 ├─ dto/
│  │  │  │                 │  ├─ ProjectDTO.java
│  │  │  │                 │  └─ UserResponseDTO.java
│  │  │  │                 │
│  │  │  │                 ├─ entity/
│  │  │  │                 │  ├─ Bookmark.java
│  │  │  │                 │  ├─ BookmarkId.java
│  │  │  │                 │  ├─ DownloadHistory.java
│  │  │  │                 │  ├─ DownloadHistoryId.java
│  │  │  │                 │  ├─ Gender.java
│  │  │  │                 │  ├─ History.java
│  │  │  │                 │  ├─ HistoryId.java
│  │  │  │                 │  ├─ Project.java
│  │  │  │                 │  ├─ Role.java
│  │  │  │                 │  └─ User.java
│  │  │  │                 │
│  │  │  │                 ├─ repository/
│  │  │  │                 │  ├─ BookmarkRepository.java
│  │  │  │                 │  ├─ DownloadHistoryRepository.java
│  │  │  │                 │  ├─ HistoryRepository.java
│  │  │  │                 │  ├─ ProjectRepository.java
│  │  │  │                 │  └─ UserRepository.java
│  │  │  │                 │
│  │  │  │                 ├─ service/
│  │  │  │                 │  ├─ DownloadHistoryService.java
│  │  │  │                 │  ├─ ProjectService.java
│  │  │  │                 │  ├─ UserCleanupService.java
│  │  │  │                 │  └─ UserService.java
│  │  │  │                 │
│  │  │  │                 └─ BackendApplication.java
│  │  │  │
│  │  │  └─ resources/
│  │  │     ├─ sql/
│  │  │     │  └─ schema.sql
│  │  │     ├─ application.properties
│  │  │     └─ application-dev.properties
│  │  │
│  │  └─ test/
│  │     └─ java/
│  │        └─ th/
│  │           └─ ac/
│  │              └─ tu/
│  │                 └─ cs/
│  │                    └─ projectportal/
│  │                       └─ BackendApplicationTests.java
│  │
│  └─ target/                       # Build output
│
├─ .gitattributes
├─ mvnw
├─ mvnw.cmd
└─ pom.xml

# Topic 2 
# Topic 3
