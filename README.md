# BITS Elevate Platform MVP UI & Interaction Specification

## Information Architecture Diagram (Textual)

- **Root Level**
  - Login Screen
  - Student Dashboard
    - Registered Courses (Course Cards)
    - Activity History
    - Notifications
    - Persistent Personas (Professor, Mentor, TA)
  - Faculty Dashboard
    - Registered Courses (Course Cards)
    - At-risk Indicators
    - Notifications
    - Persistent Personas (Professor, Mentor, TA)

- **Course Level (Student)**
  - Course Landing Page
    - 7 Modules (Tabs/Sections):
      1. Learn
      2. Reflect
      3. Practice
      4. Explore
      5. Solve
      6. Test
      7. Seek (Global, always available)
    - Course Progress
    - Resume State
    - Activity History
    - Notifications
    - Personas (Professor, Mentor, TA)

- **Course Level (Faculty)**
  - Course Overview Page
    - Content Upload & Resource Management
    - Lecture Summary Validation
    - Experiential Module Configuration
    - Workplace Problem Mapping
    - Student Insights (Risk Flags, Reflection Summaries)
    - Assessment Analytics (Concept Heatmaps)
    - AI Persona Oversight (Review-only)
    - Personas (Professor, Mentor, TA)

- **Sidebar (Both Roles)**
  - Registered Courses
  - Activity History
  - Notifications
  - Personas (Professor, Mentor, TA)

- **Global**
  - Seek Interaction (TA, Professor, Mentor, Operational Support)


## Screen Map

### Student Screens
- Login Screen
- Dashboard
  - Course Cards (with progress, resume state)
  - Activity History
  - Notifications
  - Personas (Professor, Mentor, TA)
- Course Landing Page
  - Learn Module
  - Reflect Module
  - Practice Module
  - Explore Module
  - Solve Module
  - Test Module
  - Seek Interaction (Global)

### Faculty Screens
- Login Screen
- Dashboard
  - Course Cards (with at-risk indicators)
  - Notifications
  - Personas (Professor, Mentor, TA)
- Course Overview Page
  - Content Upload & Resource Management
  - Lecture Summary Validation
  - Experiential Module Configuration
  - Workplace Problem Mapping
  - Student Insights View
  - Assessment Analytics
  - AI Persona Oversight (Review-only)


## Student UI Journey (Step-by-Step)

1. **Login Screen**
   - Username/password input
   - Privacy assurance message: "Personalization data is not visible to BITS and is deleted after graduation."
   - Login button

2. **Dashboard**
   - Student sees only registered courses as cards
   - Each card shows course progress and resume state
   - Sidebar: Activity history, notifications, personas

3. **Course Landing Page**
   - Student enters a course
   - Sees 7 modules as tabs/sections:
     - Learn: Video, timestamp summary, faculty resources, safe content sources only
     - Reflect: Guided prompts linked to Learn content, journaling, back-navigation to lecture
     - Practice: Virtual/remote labs, sandbox coding, AR/VR support, debugging hints (no direct answers)
     - Explore: Safe curated exploration beyond lecture
     - Solve: Workplace problem definition workflow, mentor-guided hypothesis refinement
     - Test: Assessments, concept weakness feedback
     - Seek: TA, Professor, Mentor, Operational Support (always available)
   - Personas (Professor, Mentor, TA) persistently visible

4. **Seek Interaction**
   - Student can access Seek at any time from any screen
   - Choose persona (TA, Professor, Mentor, Operational Support)
   - Initiate chat, request help, or schedule session


## Faculty UI Journey (Step-by-Step)

1. **Login Screen**
   - Username/password input
   - Privacy assurance message
   - Login button

2. **Dashboard**
   - Faculty sees registered courses as cards
   - Each card shows at-risk indicators
   - Sidebar: Notifications, personas

3. **Course Overview Page**
   - Faculty enters a course
   - Access:
     - Content Upload & Resource Management
     - Lecture Summary Validation
     - Experiential Module Configuration
     - Workplace Problem Mapping
     - Student Insights (risk flags, reflection summaries)
     - Assessment Analytics (concept heatmaps)
     - AI Persona Oversight (review-only)
   - Personas (Professor, Mentor, TA) persistently visible


## Navigation & Permission Matrix

| Screen/Module                | Student | Faculty | TA | Mentor | Professor | Seek | Notes |
|------------------------------|---------|---------|----|--------|-----------|------|-------|
| Login Screen                 |   X     |   X     |    |        |           |      |       |
| Dashboard                    |   X     |   X     |    |        |           |      |       |
| Course Landing Page          |   X     |   X     |    |        |           |      |       |
| Learn Module                 |   X     |   X     |    |        |           |      |       |
| Reflect Module               |   X     |   X     |    |        |           |      |       |
| Practice Module              |   X     |   X     |    |        |           |      |       |
| Explore Module               |   X     |   X     |    |        |           |      |       |
| Solve Module                 |   X     |   X     |    |        |           |      |       |
| Test Module                  |   X     |   X     |    |        |           |      |       |
| Seek Interaction             |   X     |   X     | X  |   X    |     X     |  X   | Globally available |
| Content Upload/Resource Mgmt |         |   X     |    |        |           |      | Faculty only |
| Lecture Summary Validation   |         |   X     |    |        |           |      | Faculty only |
| Experiential Module Config   |         |   X     |    |        |           |      | Faculty only |
| Workplace Problem Mapping    |         |   X     |    |        |           |      | Faculty only |
| Student Insights             |         |   X     |    |        |           |      | Faculty only |
| Assessment Analytics         |         |   X     |    |        |           |      | Faculty only |
| AI Persona Oversight         |         |   X     |    |        |           |      | Review-only |


## Persona Interaction Model

- **Persistent Personas:**
  - Professor, Mentor, TA are always visible in sidebar and course screens
  - Modeled as real human-like guides
  - Travel with learner across courses
  - Can be accessed for guidance, support, and mentoring
  - Seek interaction allows student or faculty to initiate contact with any persona at any time

- **Persona UI Presence:**
  - Sidebar: Persona avatars/names, status indicators
  - Course screens: Persona context tips, guidance prompts
  - Seek: Persona selection, chat/help interface


## Authentic–Safe–Enabling Framework (UI Reflection)

- **Authentic:**
  - All content and resources are faculty-validated
  - UI labels and resource links indicate validation status

- **Safe:**
  - Restricted web access enforced in modules (Explore, Learn)
  - Only curated, safe sources shown
  - Privacy assurance message on login

- **Enabling:**
  - AI scaffolding present in Practice, Solve, Test modules
  - Hints, feedback, and guidance provided without direct answers
  - Personas offer support, not solutions


## Strict Navigation Rules

- Course-centric architecture: All navigation flows from course selection
- Role-based access: Student and Faculty see only permitted screens/modules
- Seek is globally available from any screen
- Backend intelligence systems are invisible in UI
- No infrastructure or backend engine visibility

---

This specification strictly follows the BITS Elevate product vision and navigation rules. No alternative navigation structures or backend exposure are present. All personas, modules, and screens are mapped as required.
