# 📌 Project Proposal (Final Draft)

## 📝 Project Title  
Survey Data Collection and Response Confirmation System

---

## 🔍 Problem Statement  
This project addresses the challenge of efficiently gathering and managing feedback from respondents in educational and survey settings. Collecting comprehensive data on user satisfaction, usability, and recommendations is often disorganized or incomplete, which can lead to inaccurate conclusions. By creating a system that captures detailed respondent information and feedback, and immediately confirms submission, this project aims to improve the accuracy, organization, and reliability of survey data collection, ultimately supporting better decision-making and improvements based on user insights.  

---

## 🎯 Project Objectives  
To develop a system that accurately collects and stores respondents’ demographic information and feedback on satisfaction, usability, design, clarity, and recommendations.

To ensure the survey process is user-friendly and guides respondents smoothly throughout all questions until completion.

To implement an immediate confirmation message that notifies respondents that their responses have been successfully recorded, enhancing user confidence and engagement.

---

## ⚙️ Planned Features  
- Feature 1: Collect & record feedbacks/data from the respondents. 
- Feature 2: Mark whether a question is required or optional.
- Feature 3: Set a maximum amount of characters or words allowed in the answer.
- Feature 4: Says what kind of answer is expected (a word, number, date, etc.).
- Feature 5: Shows example text inside the answer box to guide the user. 


---

## ⌨️ Planned Inputs and Outputs  

- **Inputs**  
  - Respondent's ID number, age, gender, grade level, section, questions about satisfaction, usability, design, clarity, recommendations, and overall conclusions, and comments about the subject.
- **Outputs**  
  - Display “Your response has been recorded” at the end of the survey after the respondent has answered all of the questions.
---

## 📂 GitHub Repository Link  
Paste your GitHub repository link here:  
`https://github.com/JensineArissaOArabis/Final-Project-CS2` 

---

## LOGIC PLAN
Pseudocode:
BEGIN

START PROGRAM

LOOP forever
    DISPLAY "Survey Database Menu"
    DISPLAY options:
        1. Display All Surveys
        2. Add New Survey
        3. Update Survey
        4. Delete Survey
        5. See Features
        6. Exit

    INPUT user_choice

    IF user_choice = 1 THEN
        GET all survey data from database

        IF data exists THEN
            FOR each survey in data
                DISPLAY survey details (ID, age, gender, etc.)
            END FOR
        ELSE
            DISPLAY "No survey data found"
        END IF
    END IF


    IF user_choice = 2 THEN
        INPUT survey details:
            id, age, gender, grade level, section
            q1 to q6 (ratings 1–5)
            q7 (comments)

        CREATE survey record
        SAVE survey to database

        DISPLAY "Survey added successfully"
    END IF


    IF user_choice = 3 THEN
        INPUT survey ID to update
        FETCH survey from database

        IF survey exists THEN
            INPUT new survey details
            UPDATE survey in database
            DISPLAY "Survey updated successfully"
        ELSE
            DISPLAY "Survey not found"
        END IF
    END IF


    IF user_choice = 4 THEN
        INPUT survey ID to delete

        IF survey exists in database THEN
            DELETE survey
            DISPLAY "Survey deleted successfully"
        ELSE
            DISPLAY "Survey not found"
        END IF
    END IF


    IF user_choice = 5 THEN
        LOOP (Features Menu)
            DISPLAY feature options:
                1. Restrict comment word count
                2. Show expected answer types
                3. Planned Feature
                4. Planned Feature
                5. Planned Feature
                6. Back to Main Menu

            INPUT feature_choice

            IF feature_choice = 1 THEN
                SET max_words = 250

                LOOP
                    INPUT comment
                    COUNT words

                    IF word_count <= max_words THEN
                        DISPLAY "Accepted"
                        BREAK loop
                    ELSE
                        DISPLAY "Too many words, try again"
                    END IF
                END LOOP
            END IF


            IF feature_choice = 2 THEN
                GET sample survey data

                IF data exists THEN
                    DISPLAY expected types:
                        ID → number
                        Age → number
                        Gender → text
                        Grade Level → text
                        Section → text
                        Q1–Q6 → number (1–5)
                        Q7 → text
                ELSE
                    DISPLAY "No survey data available"
                END IF
            END IF


            IF feature_choice = 3 THEN
                DISPLAY "Planned Feature"
            END IF

            IF feature_choice = 4 THEN
                DISPLAY "Planned Feature"
            END IF

            IF feature_choice = 5 THEN
                DISPLAY "Planned Feature"
            END IF

            IF feature_choice = 6 THEN
                EXIT Features Menu
            END IF

        END LOOP
    END IF


    IF user_choice = 6 THEN
        DISPLAY "Goodbye"
        EXIT PROGRAM
    END IF


    IF input is invalid THEN
        DISPLAY "Invalid choice"
    END IF

END LOOP

END PROGRAM

END

---

## Flowchart:
<img width="1705" height="867" alt="Image" src="https://github.com/user-attachments/assets/fad410ae-d581-4a8d-ae4c-b62ccfe41dfa" />

<img width="1244" height="849" alt="Image" src="https://github.com/user-attachments/assets/b155fb99-be26-4675-900b-1dfc4be2b599" />

<img width="1706" height="872" alt="Image" src="https://github.com/user-attachments/assets/82cb7328-33da-48de-8774-ee74af460aca" />

<img width="1279" height="846" alt="Image" src="https://github.com/user-attachments/assets/044cdad6-a6c8-4913-8d6b-086b8cf32156" />

<img width="1376" height="721" alt="Image" src="https://github.com/user-attachments/assets/7908fd27-49b2-48e4-9d8b-6ea69f1c98c9" />
