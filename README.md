# MathQuest - Mathematics Learning Management System

## Contents
- [Overview](#overview)
- [How to Get Started with MathQuest](#how-to-get-started-with-mathquest)
- [Features](#features)
- [High-Level System Architecture](#high-level-system-architecture)
- [Technology Stack](#technology-stack)
- [API Endpoints](#api-endpoints)
- [Development Setup](#development-setup)
- [Test Results](#test-results)
- [Contributors / Team Members](#contributors--team-members)
- [Frequently Asked Questions](#frequently-asked-questions)
- [Help Us Improve the Project](#help-us-improve-the-project)

---

## Overview
MathQuest is an online learning management system designed to deliver math courses and curriculum in an asynchronous format, allowing students to learn at their own pace.  

**Key capabilities include:**
- Instructors: Create course offerings, design quizzes and assignments, grade student work automatically, facilitate discussions, update content.
- Students: Browse courses, register, take assessments, participate in discussions, track progress.
- Roles: Student, Instructor, and Admin with access controls.
- Architecture: Combines MVC, client-server, and microservices for scalability and modularity.

---

## How to Get Started with MathQuest

### **Student Flow**
1. Browse available courses.
2. Register for courses.
3. Access course content and assessments.
4. Participate in discussions.
5. Track progress.

### **Instructor Flow**
1. Create and publish course offerings.
2. Design quizzes and assignments.
3. Grade assessments automatically or manually.
4. Manage course discussions.

### **Admin Flow**
1. Approve/reject course requests.
2. Manage instructor accounts.
3. Moderate content.

---

## Features
- **Course Offerings and Registration**: Create and manage course listings with detailed information.
- **Course Content Management**: Add modules, quizzes, assignments, and syllabus.
- **Assessments and Grading**: Auto-graded quizzes with instant feedback.
- **Discussions**: Threaded conversations between students and instructors.
- **Role-Based Access Control**: Permissions for students, instructors, and admins.
- **Administrative Tools**: Content moderation, instructor management.

---

## High-Level System Architecture
- **Patterns Used**: MVC, client-server, and microservices.
- **Design Goals**: Scalability, modularity, and support for concurrent users.

---

## Technology Stack

| Engineering Activity        | Selected Tool(s)     |
|-----------------------------|----------------------|
| Version Control              | GitHub               |
| Development IDE              | Visual Studio Code   |
| Wireframe & UI Screens       | Balsamiq             |
| Project Planning             | Microsoft Excel      |
| Diagramming                  | LucidChart           |
| Frontend                     | React                |
| Backend                      | Node.js              |
| Database                     | MongoDB              |
| Testing                      | Jest, Karma          |

---

## API Endpoints

| Endpoint | Description | Type |
|----------|-------------|------|
| `/api/users/login` | Authenticates a user for the MathQuest system. | POST |
| `/api/users/signup` | Creates a new user for the MathQuest system. | POST |
| `/api/courses` | Gets a list of all available published courses. | POST |
| `/api/courses/teachers/getAllCourses` | Gets all courses created by a teacher. | POST |
| `/api/courses/registered/getRegisteredUsers` | Gets registered users in a specific course. | POST |
| `/api/courses/hideCourse` | Hides/unpublishes a course. | POST |
| `/api/courses/filterCoursesByStatus` | Fetches courses by request status. | POST |
| `/api/courses/changeRequestStatus` | Changes the request status of a course. | POST |
| `/api/courses/quizzes/grades/gradeQuiz` | Grades and calculates quiz points. | POST |
| `/api/courses/registered` | Gets courses a student is registered in. | POST |
| `/api/courses/registered/new` | Registers a student in a new course. | POST |
| `/api/courses/discussions/getAllThreads` | Gets all threads for a course. | POST |
| `/api/courses/discussions/getAllReplies` | Gets replies for a specific thread. | POST |
| `/api/courses/discussions/createThread` | Creates a new discussion thread. | POST |
| `/api/courses/discussions/createReply` | Creates a reply to a thread. | POST |
| `/api/courses/quizzes/getAllQuizzes` | Gets all quizzes for a course. | POST |
| `/api/courses/quizzes/getQuiz` | Gets a specific quiz with all questions and options. | POST |

---

## Development Setup

1. **Clone the Repository**
   ```bash
   git clone https://github.com/ris-tlp/mathquest.git
   cd mathquest
   code .
