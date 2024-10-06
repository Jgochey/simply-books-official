# **FE App Development Recommended Guide**

## DAY 1

1. **Create a GitHub Project Board**: 
    - [ X ] Use the Kanban template.
    - [ X ] Set up columns: Backlog, Ready, Blocked, In Progress, Testing, Done.
    - [ X ] Create tickets for each task in the project (break down features, UI components, and CRUD operations into individual tasks).

1. **Entity Relationship Diagram (ERD)**:
    - [ X ] Create an ERD to map out the relationships between books, authors, and users.
    - [ X ] Ensure all entities and relationships are clear and match Firebase’s data structure.
    - [ X ] Use tools like draw.io or Lucidchart for the ERD.
    - [ X ] If an ERD is provided, review it and ensure it fits the project needs.

1. **Project Setup**
    - [ X ] Initialize a new Next.js project.
    - [ X ] Organize the file structure for easy navigation (e.g., components, pages, utils, etc.).
    - [ X ] Install necessary dependencies (Firebase, etc.).
    - [ X ] Connect the app to Firebase (check for Google Authentication and real-time database).

1. **Authentication**
    - [ X ] Set up Firebase Authentication for Google sign-in.
    - [ X ] Ensure authentication flow works and restrict data access based on logged-in users.
    - [ X ] Test sign-in and sign-out functionality thoroughly.

1. **Routing & Navigation**
    - [ X ] Set up dynamic routing in Next.js App Router (e.g., `/books/[id]`, `/authors/[id]`).
    - [ X ] Ensure navigation between list views and individual item pages.
    - [ X ] Include links for easy navigation across the app (home, details, etc.).
    - [ X ] Test dynamic routes and ensure data loads correctly based on route params.

## DAY 2

1. **Data Management & Fetching**
    - [ X ] Create a Firebase Realtime Database or Firestore to store data (or connect to an existing one).
    - [ X ] Fetch user-specific data from Firebase (books, authors, etc.).
    - [ X ] Use `useEffect` for data fetching and ensure data renders on component mount.
    - [ X ] Test data retrieval and ensure no issues with Firebase queries.

1. **Endpoint and Database Testing with Postman**
    - [ X ] Use Postman to test all Firebase endpoints and the database.
    - [ X ] Verify the API layer works as expected (CRUD operations on books/authors).
    - [ X ] Ensure all user-specific data is correctly retrieved and updated.
    - [ X ] Check for proper authorization with Google Authentication on restricted endpoints.
    - [ X ] Document API responses and any errors to reference during development.

1. **State Management**
    - [ X ] Use `useState` for managing form inputs and component state.
    - [ X ] Ensure state is updated properly when forms are filled or events occur.
    - [ X ] Manage global or shared state using Context API or props drilling.

1. **One-to-Many Relationship with Dynamic Select Menu**
    - [ X ] Set up a **one-to-many relationship** between entities (e.g., an author can have many books).
    - [ X ] Create a form with a select menu that is dynamically populated with related options (e.g., select an author when adding/editing a book).
    - [ X ] Fetch and display the list of available options from Firebase in the select menu.
    - [ X ] Ensure the relationship is correctly reflected in the database (e.g., storing the book with its associated author ID).

## DAY 3

1. **Rendering Lists & Conditional Content**
    - [ X ] Use loops to render lists of data dynamically.
    - [ ? ] Implement conditional rendering (e.g., showing a message if no data is available).
    - [ X ] Test list rendering thoroughly with varying amounts of data.

1. **Hooks (useState, useEffect)**
    - [ X ] Implement `useState` for managing local component state.
    - [ X ] Use `useEffect` for handling side effects (e.g., data fetching).
    - [ X ] Ensure proper usage of dependencies in `useEffect` to avoid infinite loops.

1. **READ & DELETE Operations**
    - [ X ] Implement **READ**: Fetch and render lists of data (books, authors).
    - [ X ] Implement **DELETE**: Allow users to delete data from Firebase.

1. **CREATE & UPDATE Operations - Two-Way Binding & Forms**
    - [ X ] Implement **CREATE**: Build forms to add new data (e.g., books, authors) to Firebase.
    - [ X] Implement **UPDATE**: Enable editing existing data and updating it in Firebase.
    - [ X ] Implement two-way data binding in forms (real-time input reflection).
    - [ X ] Listen for input changes and update state accordingly.
    - [ X ] Ensure forms are fully functional for both creating and updating items.
    - [ X ] Ensure all CRUD operations work with user-specific data.

## DAY 4
1. README:
    - Write a detailed README file.
    - Include instructions on how to set up, run, and deploy the project.
    - Document any API usage and special features in the project.
1. Loom Video:
    - Record a 5-minute Loom video demonstrating the app.
    - Highlight key features.
    - Walk through any challenges and how they were solved.
1. Additional Documentation:
    - Provide code comments where necessary.
    - Include any diagrams or visuals explaining complex parts of the project (e.g., ERD).

## DAY 5 

1. **Deployment**
    - [ X ] Deploy the app on Netlify or another platform.
    - [ X ] Ensure the live app works as expected with all functionalities intact.
    - [ X ] Ensure all the env vars are transfered to the deployment.
    - [ X ] Share the deployed app link in the assignment submission.

## DAY 6

1. **User Experience (UX)**
    - [ ] Ensure the app is responsive and mobile-friendly.
    - [ ] Add form validation (e.g., required fields, proper formats) to enhance UX.
    - [ ] Provide clear feedback for user actions (e.g., success or error messages).

1. **Testing**
    - [ ] Test all forms (create and update) to ensure they handle input correctly.
    - [ ] Test CRUD operations for potential edge cases (e.g., deleting all items, editing invalid inputs).
    - [ ] Ensure navigation works as expected across routes.
    - [ ] Verify Google Authentication flow and access control.
