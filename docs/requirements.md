# Requirements: Internship Aggregator Platform

## 1. Roles

* Student: searches for internships, applies to them, and tracks application status
* Employer: posts internship opportunities, reviews applications, and updates status
* Admin: manages member accounts and platform reports

## 2. User stories

US-01 As a student, I want to create an account so that I can use the platform's features. [Should]
US-02 As a student, I want to view and edit my profile details so that my information is always up to date. [Could]
US-03 As a student, I want to request a password reset link so that I can regain access safely. [Must]
US-04 As a student, I want to log in using my email and password so that I can access my dashboard and apply for internships. [Must]
US-05 As a student, I want to search for internships by title or company so that I can find opportunities matching my skills. [Must]
US-06 As a student, I want to apply for an internship using my profile so that companies can review my application. [Must]
US-07 As an employer, I want to post a new internship opportunity so that students can see it and apply. [Must]
US-08 As an employer, I want to view a list of applicants for my internships so that I can choose the best candidates. [Should]
US-09 As an employer, I want to update the status of an application to Accept or Reject so that the student knows the final decision. [Must]
US-10 As a student, I want to track the status of my applications so that I know if I was accepted or rejected. [Should]
US-11 As an admin, I want to deactivate spam employer accounts so that students are protected from fake internships. [Should]
US-12 As an admin, I want a report of all active internships so that I can monitor platform growth. [Could]

## 3. Acceptance criteria

Top 5 stories. The full scenarios are in the GitHub Issues.

### US-04 User Login

```gherkin
Feature: User Login
Scenario: Successful login
Given the student is on the login page
When the student enters valid credentials
Then the student is redirected to the dashboard

Scenario: Incorrect password
Given the student is on the login page
When the student enters an incorrect password
Then the system shows an error "Invalid email or password"
```

### US-05 Search for Internships

```gherkin
Feature: Search Internships
Scenario: Search returns matching results
Given the platform has an internship titled "AI Engineer"
When the student searches for "AI"
Then the results include the "AI Engineer" internship

Scenario: Search finds nothing
Given the platform has no internships for "Dentist"
When the student searches for "Dentist"
Then the student sees the message "No internships found"
```

### US-06 Apply for an Internship

```gherkin
Feature: Apply for Internship
Scenario: Successful application
Given a student has a complete profile with a resume
And an internship is "Open"
When the student clicks "Apply"
Then the application is submitted successfully

Scenario: Apply with incomplete profile
Given a student has no resume uploaded
When the student tries to apply
Then the request is rejected with "Please upload a resume first"
```

### US-07 Post a New Internship

```gherkin
Feature: Post Internship
Scenario: Employer posts a valid internship
Given the employer is on the "New Internship" page
When the employer enters title and description
Then the internship is published and visible to students

Scenario: Missing title
Given the employer is on the "New Internship" page
When the employer submits the form without a title
Then the request is rejected with "Title is required"
```

### US-09 Update Application Status

```gherkin
Feature: Update Status
Scenario: Accept an applicant
Given a pending application exists
When the employer clicks "Accept"
Then the application status changes to "Accepted"

Scenario: Cannot update closed internship
Given an internship is marked as "Closed"
When the employer tries to change an applicant's status
Then the action is blocked with "Internship is already closed"
```

## 4. Non-functional requirements

* NFR-01 (Performance) Search returns results in < 2 s for 10,000 internships. [Should]
* NFR-02 (Security) Passwords are stored hashed (bcrypt, cost >= 12). [Must]
* NFR-03 (Usability) A new student completes a first application in under 3 minutes without help. [Should]
* NFR-04 (Availability) The system is available 99% of the time, measured monthly. [Could]

## 5. MVP scope

Must stories in the MVP: US-03, US-04, US-05, US-06, US-07, US-09
Must NFR in the MVP: NFR-02
Reason: Together they let an employer post internships, students search and apply for them securely, and employers update the application status. The Should and Could stories stay in the backlog.
