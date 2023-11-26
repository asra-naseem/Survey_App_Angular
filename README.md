
# Campus Visit Feedback Survey Application

## Project Overview
The Campus Visit Feedback Survey Application is designed to collect and display feedback from
prospective students about their campus visits at George Mason University's School of Computing. This
is an end-to-end full-stack web application with the front-end built with Angular 14 and the back-end
using Java Spring Bootx and JPA with MySQL Workbench for database management.

## Technology Stack
- **Frontend**: Angular 14, HTML5, CSS3
- **Backend**: Java Spring Boot, JPA (Java Persistence API)
- **Database**: MySQL Workbench

## Frontend Architecture
### Components
#### 1. AppComponent (Root Component)
- **Purpose**: Serves as the root of the application, containing global components like the
navigation bar and router-outlet.
- **Template**: app.component.html provides the structure for the navigation bar with links
to the main areas of the application and includes the <router-outlet> directive, which is
the placeholder for rendering the active component based on the URL route.
- **Logic**: app.component.ts initializes the application. It can also be used to handle global
logic such as authentication checks or theme settings.

#### 2. HomeComponent (Landing Page)
- **Purpose**: Acts as the landing page, providing a welcoming introduction and detailed
information about George Mason University's School of Computing.
- **Template**: home.component.html includes headings, paragraphs, and styling to present
the university's content in an engaging format. It is designed to be visually appealing and
informative, using inline styles to adhere to the university's brand guidelines.
- **Logic**: home.component.ts is typically straightforward for a static home page, primarily
handling initialization routines. Additional logic can be included if dynamic content or
interactivity is required on the home page.

#### 3. StudentSurveyComponent (Survey Form Handler)
- **Purpose**: Manages the collection of survey data from prospective students with a form-
based interface.
- **Template**: StudentSurvey.component.html contains the HTML form with input fields for
personal details, survey questions, and submission controls. It uses Angular’s form
directives to bind form controls to the component's logic and to manage validation and
form state.
- **Logic**: StudentSurvey.component.ts creates and manages the form model using
Angular’s reactive forms API. It defines form controls, validation rules, and methods for
handling form submissions, including interactions with SurveyService to submit the data
to the backend.

#### 4. ListComponent (Survey Data Display)
- **Purpose**: Displays a list of all surveys that have been submitted.
