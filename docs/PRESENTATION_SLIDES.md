# 📊 Library Management System - Presentation Slides
## Capstone Project Presentation

---

## Slide 1: Title Slide
**Library Management System (LMS) - Capstone Project**
*Full Stack Web Development Project*

**Presented by:** Teo Yong Song  
**Date:** 3rd October 2025  

**Presentation Hints:**
- Briefly introduce yourself and the project
- Mention that the LMS is a web application designed to streamline library operations and enhance user experience

---

## Slide 2: Project Overview
### Library Management System

**About the Project:**
- Web application for managing library operations
- Two main user roles: Librarian (Admin) and Member
- Built using Spring Boot (Backend), React (Frontend), and MySQL (Database)

**Presentation Hints:**
- Explain the purpose of the LMS
- Highlight the two user roles and their functionalities
- Mention the technologies used

---

## Slide 3: Project Goals
### Development Objectives

**Project Goals:**
- Develop a fully functional web application
- Enable librarians to manage books and members efficiently
- Provide a user-friendly interface for members to search for books and track borrowing history
- Create a robust and scalable system

**Presentation Hints:**
- Emphasize the importance of creating a functional and scalable system
- Mention the focus on user experience for both librarians and members

---

## Slide 4: Key Features
### Core Functionality

**Key Features:**
- **User Management:** Registration, login, profile management, password reset
- **Member Management:** Register, edit, delete, and search members
- **Book Management:** Add, update, delete, and search books
- **Lending Management:** Borrow, return, reserve books, and track due dates

**Presentation Hints:**
- Briefly explain each feature
- Highlight how these features will improve library operations

---

## Slide 5: Business Rules
### System Rules and Policies

**Membership Rules:**
- Maximum 3 books per member
- 1-year membership validity
- Valid membership required for borrowing

**Lending Rules:**
- 14-day loan period
- Maximum 2 renewals allowed
- No borrowing if overdue books exist
- No borrowing if fines exceed $10

**Fine Calculation:**
- $0.50 per day for overdue books
- Maximum $20 fine per book

**Presentation Hints:**
- Explain the rules governing memberships and lending
- Mention how fines are calculated

---

## Slide 6: Technical Requirements
### Technology Stack

**Backend Technologies:**
- Spring Boot framework
- RESTful API design
- MySQL database
- Spring Security (planned)
- JPA/Hibernate for ORM

**Frontend Technologies:**
- React.js with hooks
- React Router for navigation
- Bootstrap/Material-UI for styling
- Axios for API communication

**Database Requirements:**
- Proper relationship mapping
- Referential integrity
- Database indexing
- Data validation

**Presentation Hints:**
- Highlight the technologies used for backend, frontend, and database
- Mention the importance of security and data integrity

---

## Slide 7: System Architecture
### MVC Architecture Implementation

**Architecture Type:** Model-View-Controller (MVC)

**MVC Implementation:**
- **Model:** JPA Entities (User, Book, Borrowing)
- **View:** React Components (UI Layer)
- **Controller:** Spring Boot REST Controllers

**Benefits of MVC:**
- Separation of concerns
- Maintainable code structure
- Scalable architecture
- Easy testing and debugging

**Presentation Hints:**
- Describe how MVC helped in system implementation
- Explain the separation of concerns

---

## Slide 8: Screenshots of Key Features
### System Interface Overview

**Admin Portal Features:**
- User Management Dashboard
- Book Management Interface
- System Analytics and Reports
- Overdue Notifications

**Member Portal Features:**
- Book Search and Browse
- Personal Borrowing History
- Profile Management
- Due Date Tracking

**Presentation Hints:**
- Describe role of each portal
- Talk about various features supported under each portal
- Show actual screenshots of the running application

---

## Slide 9: Database & System Designs
### Entity Relationship and System Flow

**Database Design:**
- **ERD Screenshot:** Show entity relationships
- **Main Entities:** Users, Books, Borrowings
- **Relationships:** One-to-Many between Users-Borrowings and Books-Borrowings

**System Flow Design:**
- **Wireframe/Prototype:** Overall Library System flow
- **User Registration Flow:** Registration → Login → Dashboard
- **Borrowing Flow:** Search → Select → Borrow → Track → Return

**Presentation Hints:**
- Describe main entities and relationships
- With wireframes/prototype explain the flow of the system

---

## Slide 10: API Endpoints
### RESTful API Documentation

**Admin Endpoints:**
- `GET /api/users` - Get all users
- `POST /api/users` - Create new user
- `PUT /api/users/{id}` - Update user
- `DELETE /api/users/{id}` - Delete user
- `GET /api/books` - Get all books
- `POST /api/books` - Add new book
- `PUT /api/books/{id}` - Update book
- `DELETE /api/books/{id}` - Delete book

**Member Endpoints:**
- `GET /api/books/search` - Search books
- `GET /api/borrowings/user/{userId}` - Get user borrowings
- `POST /api/borrowings` - Borrow a book
- `PUT /api/borrowings/return/{id}` - Return a book

**Authentication Endpoints:**
- `POST /api/auth/login` - User login
- `POST /api/users/register` - User registration

**Presentation Hints:**
- Mention the endpoints used by admin and members
- Explain CRUD operations available for each role

---

## Slide 11: Test Cases - UATs
### User Acceptance Testing

**Functional UATs Implemented:**
- **User Management Testing:** Registration, login, profile updates
- **Book Management Testing:** Add, edit, delete, search books
- **Borrowing System Testing:** Borrow, return, overdue tracking
- **Authentication Testing:** Role-based access control

**Test Scenarios:**
- Valid user registration and login
- Invalid credentials handling
- Book availability checking
- Overdue book notifications
- Profile update functionality

**Screenshots:** Test execution results and outputs

**Presentation Hints:**
- Talk about how tests are carried out for user registration, login, etc.
- Show screenshots of test results

---

## Slide 12: Challenges and Solutions
### Development Challenges Overcome

**Challenges Encountered:**
- **Frontend-Backend Integration:** API communication and data flow
- **Role-based Access Control:** Implementing proper authentication
- **Fine Calculation Logic:** Handling overdue books and penalties
- **Data Validation:** Ensuring data integrity and security

**Solutions Implemented:**
- **API Integration:** Used Axios for reliable HTTP communication
- **Authentication:** Implemented JWT-based authentication system
- **Business Logic:** Created service layer for complex calculations
- **Validation:** Used Bean Validation for input sanitization

**Presentation Hints:**
- Discuss the challenges encountered during the project
- Explain how these challenges were overcome

---

## Slide 13: Future Enhancements
### Planned Improvements

**Mobile App Integration:**
- React Native mobile application
- Cross-platform compatibility
- Offline functionality

**Advanced Features:**
- Advanced search with filters
- Book recommendation system
- Integration with external libraries
- Enhanced reporting and analytics

**System Improvements:**
- Real-time notifications
- Email integration
- Advanced user analytics
- Multi-library support

**Presentation Hints:**
- Discuss potential future improvements to the LMS
- Mention how these enhancements could further improve the system

---

## Slide 14: Conclusion
### Project Summary and Achievements

**Project Summary:**
- Successfully developed a full-stack Library Management System
- Implemented all core features for both admin and member roles
- Created a scalable and maintainable architecture
- Delivered a user-friendly interface with modern design

**Key Achievements:**
- ✅ Complete CRUD operations for all entities
- ✅ Role-based authentication and authorization
- ✅ Responsive design for all devices
- ✅ Comprehensive API documentation
- ✅ Database optimization and security
- ✅ User acceptance testing completed

**Technical Skills Demonstrated:**
- Full-stack web development
- Database design and optimization
- API development and integration
- Modern UI/UX design principles
- Testing and quality assurance

**Q&A Session**

---

## Presentation Notes

### Timing Breakdown (15 minutes total):
- **Introduction & Overview:** 2 minutes
- **Goals & Features:** 3 minutes
- **Technical Implementation:** 4 minutes
- **Screenshots & Demo:** 4 minutes
- **Challenges & Future:** 2 minutes

### Demo Preparation:
1. Have the system running locally (Backend: http://localhost:8080, Frontend: http://localhost:5174)
2. Prepare sample data (books, users, borrowings)
3. Practice the demo flow for both admin and member roles
4. Have backup screenshots ready
5. Test all features beforehand

### Key Points to Emphasize:
- Full-stack development capabilities
- Modern technology stack implementation
- User-centered design approach
- Scalable and maintainable architecture
- Production-ready code quality

### Screenshots to Include:
- Login page with role selection
- Admin dashboard with statistics
- Book management interface
- Member book search page
- Borrowing history page
- Profile management page
- Database ERD diagram
- API endpoint documentation

### Potential Questions:
- How does the system handle concurrent users?
- What security measures are implemented?
- How would you deploy this to production?
- What testing methodologies were used?
- How does the system scale with more data?

---


**Presentation Slides** - Library Management System Capstone Project 📊🎯
