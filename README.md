# EHAS - Exam Hall Allocation System

**EHAS** is a comprehensive, real-time distributed system designed to streamline the management of examination halls, seating arrangements, and invigilation duties. It features three distinct desktop applications for Administrators, Teachers, and Students, all synchronized instantly via a central Node.js server.

## 🚀 Key Features

*   **Real-time Synchronization**: Powered by **Socket.io**, changes made by administrators (like seat allocation) are instantly reflected on student and teacher dashboards without page reloads.
*   **Role-Based Applications**:
    *   **Admin App (EHAS)**: Full control over exam scheduling, room creation, student/staff management, and visual seating allocation.
    *   **Teacher App**: tailored view for invigilators to see their assigned duties and exam details.
    *   **Student App**: Allows students to check their exam schedule and assigned seat/room location.
*   **Visual Seating Management**: Interactive tools to allocate students to specific seats within exam halls.
*   **Secure & Lightweight**: Built with **Tauri**, providing native desktop application performance with a tiny memory footprint compared to Electron.

## 🛠 Tech Stack

*   **Frontend (Desktop Apps)**:
    *   [Tauri](https://tauri.app/) (v2)
    *   [React](https://react.dev/) + [Vite](https://vitejs.dev/)
    *   [Ant Design](https://ant.design/) (UI Component Library)
*   **Backend (API)**:
    *   [Node.js](https://nodejs.org/) & [Express.js](https://expressjs.com/)
    *   [Socket.io](https://socket.io/) (Real-time communication)
    *   [MongoDB](https://www.mongodb.com/) & [Mongoose](https://mongoosejs.com/) (Database)

## 📂 Project Structure

*   `backend/` - Central Express.js API & WebSocket server.
*   `EHAS/` - Main Administrator Desktop Application.
*   `EHAS_teacher/` - Teacher/Invigilator Application.
*   `EHAS_student/` - Student Application.

## 🏁 Getting Started

### Prerequisites
*   Node.js (LTS version)
*   Rust (required for building Tauri apps)
*   MongoDB instance

### Installation

1.  **Clone the repository**
    ```bash
    git clone https://github.com/yourusername/EHAS.git
    cd EHAS
    ```

2.  **Setup Backend**
    ```bash
    cd backend
    npm install
    # Create a .env file with your MONGODB_URI
    npm start
    ```

3.  **Run Clients (e.g., Admin App)**
    ```bash
    cd EHAS
    npm install
    npm run tauri dev
    ```

## 📄 License
This project is licensed under the ISC License.
