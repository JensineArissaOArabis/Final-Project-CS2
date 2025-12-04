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

    DISPLAY "Welcome to the Survey Data Collection System"

    // PROMPT "Enter your ID number: "
    READ id_number

    PROMPT "Enter your age: "
    READ age

    PROMPT "Enter your gender: "
    READ gender

    PROMPT "Enter your grade level: "
    READ grade_level

    PROMPT "Enter your section: "
    READ section

    // Collect survey feedback
    DISPLAY "Rate the following from 1 (Poor) to 5 (Excellent):"

    PROMPT "Satisfaction: "
    READ satisfaction_rating

    PROMPT "Usability: "
    READ usability_rating

    PROMPT "Design: "
    READ design_rating

    PROMPT "Clarity: "
    READ clarity_rating

    PROMPT "Recommendations (Yes/No): "
    READ recommendation_answer

    PROMPT "Overall conclusion (short answer): "
    READ conclusion_text

    PROMPT "Additional comments about the subject: "
    READ comment_text

    // Store all data
    CREATE survey_record

    SET survey_record.id_number = id_number
    SET survey_record.age = age
    SET survey_record.gender = gender
    SET survey_record.grade_level = grade_level
    SET survey_record.section = section
    SET survey_record.satisfaction_rating = satisfaction_rating
    SET survey_record.usability_rating = usability_rating
    SET survey_record.design_rating = design_rating
    SET survey_record.clarity_rating = clarity_rating
    SET survey_record.recommendation = recommendation_answer
    SET survey_record.conclusion = conclusion_text
    SET survey_record.comments = comment_text

    SAVE survey_record TO dataset

    // Confirmation output
    DISPLAY "Your response has been recorded"

END

---

## Flowchart:
