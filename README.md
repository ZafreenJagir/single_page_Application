# Single Page Application (SPA) Using React Router
## Workflow of the Application
1️⃣ App Starts → Main Router Loads

When the React app starts:

App.jsx loads

<Router> starts managing the URLs

<AuthProvider> initializes login state (isLogged = false)

2️⃣ User visits Home Page (/)

On opening the app (http://localhost:5173
):

User sees Home Page

Links available:

Login

Dashboard

👉 If user clicks Dashboard before logging in → they will be redirected to Login.

3️⃣ User goes to Login Page (/login)

On the login page:

User clicks the Login button

The app runs:

setIsLogged(true);
navigate("/dashboard");


→ This marks the user as logged in
→ Redirects to Dashboard

4️⃣ ProtectedRoute checks login status

When user tries to open /dashboard:

ProtectedRoute logic:
If logged in → allow access (show dashboard)
If not logged in → redirect to /login

## OUTPUT:

<img width="779" height="719" alt="image" src="https://github.com/user-attachments/assets/47dce9cf-e8b9-47b3-b42a-00059696b3eb" />

<img width="862" height="536" alt="image" src="https://github.com/user-attachments/assets/ba4cd096-6e7e-43bc-8afe-20250ac0a0e0" />


<img width="697" height="449" alt="image" src="https://github.com/user-attachments/assets/49a42f73-c039-40f5-89dc-21b6c6e2a51a" />


<img width="857" height="503" alt="image" src="https://github.com/user-attachments/assets/7243f2c9-af47-4850-9851-a315d42d5ea8" />
