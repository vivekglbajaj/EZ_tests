A modern and visually dynamic frontend web application built for EZ Labs Assessment — showcasing animations, real API integration, and a clean modular React architecture.

**Live Project:** https://animated-cobbler-9bbe9f.netlify.app/
**GitHub Repository:** https://github.com/vivekglbajaj/EZ_tests.git

---

## 🧭 System Design & Project Flow

### 🏗️ **1. High-Level Design (HLD)**

The architecture follows a **component-based modular design**, ensuring separation of concerns, reusability, and scalability.

#### ⚙️ Architecture Overview
---

#### 🧱 HLD Diagram
+-----------------------------------------------------+

FRONTEND (React)
UI Layer (Tailwind + Framer Motion)
State Mgmt (Context API)
Routing (React Router DOM)
API Integration (Axios)
+-----------------------------------------------------+

BACKEND (EZ Labs API)
Endpoint: https://vernanbackend.ezlab.in/api/contact-us/

Handles: POST requests for contact submissions
Validates input, stores message, returns JSON
+-----------------------------------------------------+


This setup ensures that the **frontend is completely decoupled** from backend logic — allowing rapid UI iteration while maintaining reliable data communication.

---

### 🧩 **2. Low-Level Design (LLD)**

#### 📂 Component Responsibilities
| Component | Responsibility |
|------------|----------------|
| `Navbar.jsx` | Fixed top navigation bar with theme toggle |
| `HeroSection.jsx` | Landing section with motion-based intro |
| `Services.jsx` | Displays Film, Branding, and Art cards with hover tilt animations |
| `AboutSection.jsx` | Displays brand statistics, quote, and client info |
| `AboutTeam.jsx` | Interactive team showcase with animated silhouettes |
| `ContactForm.jsx` | Functional form integrated with EZ Labs API |
| `ThemeContext.jsx` | Manages dark/light mode globally |

#### 🧠 Flow of Operations
1. **User visits** the homepage → smooth scroll animations activate (Framer Motion).
2. **Navigates to a service page** (Film/Brand/Art) → new route renders content dynamically.
3. **Visits Contact Form** → fills in details (all frontend validations applied).
4. **Form submission** → triggers POST request via Axios.
5. **Response 200 OK** → toast or message “Form Submitted Successfully”.
6. **Invalid fields** → frontend validation prevents submission.

---
🧭 **Project Flow**
1️⃣ User visits the landing page → Hero section animation triggers.  
2️⃣ Scroll to Services → Hover cards animate and tilt on motion.  
3️⃣ About section → Overlapping stat cards appear with smooth motion.  
4️⃣ Team section → Animated silhouettes and call-to-action.  
5️⃣ Contact form → User submits → API call → Success message shown.  


## 🌟 Features Implemented

- ✅ **Modern UI with motion effects**
- ✅ **Fully responsive for all devices**
- ✅ **Real API integration** (`https://vernanbackend.ezlab.in/api/contact-us/`)
- ✅ **Frontend form validation (name, email, phone, message)**
- ✅ **Dynamic dark/light theme**
- ✅ **Animated icons & gradients**
- ✅ **Role-based storytelling for team section**
- ✅ **Creative 3D-like overlapping layouts**
- ✅ **Performance optimized**

---

## 🧠 Key Design Choices

| Aspect | Approach |
|--------|-----------|
| **Styling** | Tailwind CSS for utility-first rapid design |
| **Animation** | Framer Motion for smooth transitions |
| **State Management** | Context API for theme control |
| **API Integration** | Axios for structured error handling |
| **Routing** | React Router DOM (client-side navigation) |
| **Validation** | Regex-based checks for form inputs |
| **Responsiveness** | Mobile-first grid and flex architecture |

---

## 🧾 API Integration

### Endpoint:

🛠️ Installation & Setup
# Clone repository
git clone https://github.com/vivekglbajaj/EZ_TEST.git

# Navigate into folder
cd ezlabs-homepage

# Install dependencies
npm install

# Start local development
npm run dev


App runs on → http://localhost:5173

🧪 API Testing (Postman)
Field	Value
Method	POST
URL	https://vernanbackend.ezlab.in/api/contact-us/

Headers	Content-Type: application/json
Body	{ "name": "Vivek", "email": "vivek@gmail.com", "phone": "9876543210", "message": "Testing API" }

<img width="1039" height="757" alt="Screenshot 2025-11-09 at 3 07 22 PM" src="https://github.com/user-attachments/assets/a9255a05-b263-417a-9572-1c5a4c714813" />

## 🧑‍💻 Author
**Vivek Kumar Yadav**  
Frontend Developer | React.js | Java | UI/UX Design  

🔗 **Portfolio:** [LinkedIn](https://linkedin.com/in/vivek-yadav)  
💻 **GitHub:** [github.com/vivekglbajaj](https://github.com/vivekglbajaj)
