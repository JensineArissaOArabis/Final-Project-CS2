# 📌 Project Proposal (Draft)

## 📝 Project Title  
Survey Data Collection and Response Confirmation System

---

## 🔍 Problem Statement  
This project addresses the challenge of efficiently gathering and managing feedback from respondents in educational or survey settings. Often, collecting comprehensive data on user satisfaction, usability, and recommendations can be disorganized or incomplete, leading to inaccurate conclusions. By creating a system that captures detailed respondent information and feedback, and immediately confirms submission, this project aims to improve the accuracy, organization, and reliability of survey data collection, ultimately supporting better decision-making and improvements based on user insights.  

---

## 🎯 Project Objectives  
To develop a system that accurately collects and stores respondents’ demographic information and feedback on satisfaction, usability, design, clarity, and recommendations.

To ensure the survey process is user-friendly and guides respondents smoothly through all questions until completion.

To implement an immediate confirmation message that notifies respondents their responses have been successfully recorded, enhancing user confidence and engagement.

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

    DISPLAY "Welcome to the Survey Data Collection System"

    // Collect demographic information
    PROMPT "Enter your full name: "
    READ name

    PROMPT "Enter your age: "
    READ age

    PROMPT "Enter your email: "
    READ email

    PROMPT "Enter your occupation: "
    READ occupation

    // Collect survey feedback
    DISPLAY "Rate the following from 1 (Poor) to 5 (Excellent):"

    PROMPT "Overall satisfaction: "
    READ satisfaction_rating

    PROMPT "System usability: "
    READ usability_rating

    PROMPT "Question clarity: "
    READ clarity_rating

    PROMPT "Design and layout: "
    READ design_rating

    PROMPT "Would you recommend this system? (Yes/No): "
    READ recommendation

    // Store all data
    CREATE survey_record
    SET survey_record.name = name
    SET survey_record.age = age
    SET survey_record.email = email
    SET survey_record.occupation = occupation
    SET survey_record.satisfaction_rating = satisfaction_rating
    SET survey_record.usability_rating = usability_rating
    SET survey_record.clarity_rating = clarity_rating
    SET survey_record.design_rating = design_rating
    SET survey_record.recommendation = recommendation

    SAVE survey_record TO dataset

    // Confirmation message
    DISPLAY "Thank you! Your responses have been recorded."

END

---

## Flowchart:
