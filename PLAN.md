# Sprint Plan — Enrollment Helpdesk Assistant

## Project Goal
Build a mobile-friendly chatbot for the fictional Bayanihan College that answers enrollment questions using only the school's FAQ, predicts each question's category with a trained machine-learning model, and admits when the available information does not contain an answer.

## User Stories

### 1. Incoming Freshman
**User story:** As an incoming freshman, I want to ask enrollment questions in English or Filipino so that I can understand the requirements, schedule, payment options, and scholarship information.

**Acceptance criteria**
- Given a question covered by the FAQ, when I send it, the assistant returns an answer grounded only in the relevant FAQ entries and displays the IDs of the entries used.
- Given a question that is not covered by the FAQ, when I send it, the assistant clearly says it does not know and directs me to confirm the information with the registrar.

### 2. Parent or Guardian
**User story:** As a parent or guardian, I want to check general enrollment and payment information so that I can help my child prepare for enrollment.

**Acceptance criteria**
- Given a question about a documented payment option or enrollment requirement, when I ask it, the assistant answers using the official FAQ content provided for this fictional school.
- Given a request for a student's private information, when I send it, the assistant does not reveal or invent grades, records, or other personal information.

### 3. Registrar Staff
**User story:** As a registrar staff member, I want to review question categories and user feedback so that I can identify common enrollment concerns and improve the FAQ.

**Acceptance criteria**
- Given that users have submitted questions and ratings, when I open the admin page, I can view question counts by predicted category and the percentage of positive ratings.
- Given a user's message, when the assistant processes it, the system records the predicted category and any submitted thumbs-up/thumbs-down rating without storing unnecessary sensitive personal information.

## Task Backlog

| Task | Status |
|---|---|
| Create repository and set up Python dependencies | To Do |
| Write at least 15 consistent FAQ entries across five categories | To Do |
| Implement Flask chat endpoint with input validation and top-3 FAQ retrieval | To Do |
| Connect Gemini using an environment variable and a grounded prompt | To Do |
| Create 50 labeled English/Filipino intent examples | To Do |
| Train and evaluate the scikit-learn intent classifier | To Do |
| Build mobile-friendly chat interface and feedback controls | To Do |
| Add chat logging, `/api/stats`, and `/admin` dashboard | To Do |
| Test normal, off-topic, prompt-injection, privacy, and unsupported questions | To Do |
| Deploy to Render and test on a phone | To Do |
| Complete ethics reflection and submission recording | To Do |

## Backlog Update
**Current status:** Part A planning completed. The remaining tasks are marked **To Do** because implementation and testing have not yet been completed.
