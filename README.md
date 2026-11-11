ollama_helper.py
import ollama

def ask_ollama(prompt):
    response = ollama.chat(
        model="qwen2.5:3b",
        messages=[
            {"role": "user", "content": prompt}
        ]
    )
    return response["message"]["content

    pip install ollama
    ollama pull qwen2.5:3b
     ollama serve
     
    
1. Grammar Correction Assistant
File: q1_grammar.py
from ollama_helper import ask_ollama

text = input("Enter a sentence: ")

prompt = f"Correct all grammar and spelling mistakes:\n{text}"

answer = ask_ollama(prompt)

print("\nCorrected Text:", answer)

with open("corrected_text.txt", "w") as f:
    f.write(answer)

  2. Sentiment Analysis
File: q2_sentiment.py
from ollama_helper import ask_ollama

text = input("Enter a review: ")

prompt = f"Analyze the sentiment as Positive, Negative or Neutral:\n{text}"

answer = ask_ollama(prompt)

print("\nSentiment:", answer)

with open("sentiment.txt", "w") as f:
    f.write(answer)
3. MCQ Generator
File: q3_mcq.py
from ollama_helper import ask_ollama

topic = input("Enter the topic: ")
n = input("Enter number of questions: ")

prompt = f"Generate {n} multiple choice questions on {topic} with four options and answers."

answer = ask_ollama(prompt)

print("\nMCQ Questions:\n", answer)

with open("mcq.txt", "w") as f:
    f.write(answer)

    4. Study Assistant
File: q4_study.py
from ollama_helper import ask_ollama

topic = input("Enter the topic: ")

prompt = f"Act as a study assistant. Explain {topic} in simple language with examples."

answer = ask_ollama(prompt)

print("\nStudy Notes:\n", answer)

with open("study_notes.txt", "w") as f:
    f.write(answer)
5. Flashcard Generator
File: q5_flashcard.py
from ollama_helper import ask_ollama

topic = input("Enter the topic: ")

prompt = f"Create 10 flashcards for {topic} with questions and answers."

answer = ask_ollama(prompt)

print("\nFlashcards:\n", answer)

with open("flashcards.txt", "w") as f:
    f.write(answer)
    6. Meeting Minutes Generator
File: q6_meeting.py
from ollama_helper import ask_ollama

text = input("Enter meeting discussion: ")

prompt = f"Prepare meeting minutes including decisions, key points and action items:\n{text}"

answer = ask_ollama(prompt)

print("\nMeeting Minutes:\n", answer)

with open("meeting_minutes.txt", "w") as f:
    f.write(answer)
7. Resume Analyzer
File: q7_resume.py
from ollama_helper import ask_ollama

resume = input("Enter your resume details: ")

prompt = f"Analyze this resume. Identify skills, strengths, weaknesses and suggestions:\n{resume}"

answer = ask_ollama(prompt)

print("\nResume Analysis:\n", answer)

with open("resume_analysis.txt", "w") as f:
    f.write(answer)

    8. College FAQ Chatbot
File: q8_college_faq.py
from ollama_helper import ask_ollama

print("WELCOME TO COLLEGE FAQ CHATBOT")

while True:
    question = input("\nAsk a question (exit to stop): ")

    if question.lower() == "exit":
        break

    prompt = f"Act as a college FAQ chatbot. Answer this question clearly:\n{question}"

    answer = ask_ollama(prompt)

    print("\nChatbot:", answer)

  9. Feedback Analyzer
File: q9_feedback.py
from ollama_helper import ask_ollama

feedback = input("Enter customer feedback: ")

prompt = f"Analyze this feedback. Identify positive points, negative points and suggestions:\n{feedback}"

answer = ask_ollama(prompt)

print("\nFeedback Analysis:\n", answer)

with open("feedback_analysis.txt", "w") as f:
    f.write(answer)

    10. Interview Preparation Assistant
File: q10_interview.py
from ollama_helper import ask_ollama

role = input("Enter job role: ")

prompt = f"Generate 10 interview questions and answers for the job role {role}."

answer = ask_ollama(prompt)

print("\nInterview Preparation:\n", answer)

with open("interview_questions.txt", "w") as f:
    f.write(answer)

    11. Story Generator
File: q11_story.py
from ollama_helper import ask_ollama

topic = input("Enter story topic: ")

prompt = f"Generate a creative and interesting short story about {topic}."

answer = ask_ollama(prompt)

print("\nGenerated Story:\n", answer)

with open("story.txt", "w") as f:
    f.write(answer)
 12. Language Translation
File: q12_translation.py   
from ollama_helper import ask_ollama

text = input("Enter text: ")
language = input("Enter target language: ")

prompt = f"Translate the following text into {language}:\n{text}"

answer = ask_ollama(prompt)

print("\nTranslated Text:", answer)

with open("translated_text.txt", "w") as f:
    f.write(answer)
    
    13. Text Summarizer
File: q13_summarizer.py
from ollama_helper import ask_ollama

text = input("Enter a paragraph: ")

prompt = f"Summarize the following text into simple and short points:\n{text}"

answer = ask_ollama(prompt)

print("\nSummary:\n", answer)

with open("summary.txt", "w") as f:
    f.write(answer)

    14. Question Paper Generator
File: q14_question_paper.py
from ollama_helper import ask_ollama

subject = input("Enter subject: ")
topic = input("Enter topic: ")

prompt = f"Generate a question paper for {subject} on {topic} with 2-mark, 5-mark and 10-mark questions."

answer = ask_ollama(prompt)

print("\nQuestion Paper:\n", answer)

with open("question_paper.txt", "w") as f:
    f.write(answer)
15. Paragraph Rewriter
File: q15_rewriter.py
from ollama_helper import ask_ollama

text = input("Enter paragraph: ")

prompt = f"Rewrite this paragraph in clear and simple English without changing its meaning:\n{text}"

answer = ask_ollama(prompt)

print("\nRewritten Paragraph:\n", answer)

with open("rewritten_text.txt", "w") as f:
    f.write(answer)
16. Keyword Extractor
File: q16_keywords.py
from ollama_helper import ask_ollama

text = input("Enter text: ")

prompt = f"Extract the important keywords from this text:\n{text}"

answer = ask_ollama(prompt)

print("\nKeywords:\n", answer)

with open("keywords.txt", "w") as f:
    f.write(answer)
    17. Assignment Topic Generator
File: q17_assignment.py
from ollama_helper import ask_ollama

subject = input("Enter subject: ")

prompt = f"Generate 10 interesting assignment topics for {subject} with short descriptions."

answer = ask_ollama(prompt)

print("\nAssignment Topics:\n", answer)

with open("assignment_topics.txt", "w") as f:
    f.write(answer)
18. Product Description Generator
File: q18_product.py
from ollama_helper import ask_ollama

product = input("Enter product name: ")

prompt = f"Generate an attractive product description for {product} including features and benefits. Do not invent specifications."

answer = ask_ollama(prompt)

print("\nProduct Description:\n", answer)

with open("product_description.txt", "w") as f:
    f.write(answer)

    19. Daily Task Planner
File: q19_task_planner.py

from ollama_helper import ask_ollama

tasks = input("Enter your daily tasks: ")

prompt = f"Create a daily timetable and prioritize these tasks:\n{tasks}"

answer = ask_ollama(prompt)

print("\nDaily Task Plan:\n", answer)

with open("daily_plan.txt", "w") as f:
    f.write(answer)

    20. Interview Assistant
File: q20_interview_assistant.py
from ollama_helper import ask_ollama

question = input("Enter interview question: ")

prompt = f"Act as an interview assistant. Give a clear and professional sample answer:\n{question}"

answer = ask_ollama(prompt)

print("\nSuggested Answer:\n", answer)

with open("interview_answer.txt", "w") as f:
    f.write(answer)
    
    21. Grammar Correction Assistant
File: q21_grammar.py
from ollama_helper import ask_ollama

text = input("Enter text: ")

prompt = f"Correct grammar and spelling mistakes:\n{text}"

answer = ask_ollama(prompt)

print("\nCorrected Text:", answer)

with open("corrected_text.txt", "w") as f:
    f.write(answer)

    22. Sentiment Analysis
File: q22_sentiment.py
from ollama_helper import ask_ollama

text = input("Enter customer review: ")

prompt = f"Identify whether the sentiment is Positive, Negative or Neutral:\n{text}"

answer = ask_ollama(prompt)

print("\nSentiment:", answer)

with open("sentiment.txt", "w") as f:
    f.write(answer)

    23. MCQ Generator
File: q23_mcq.py

    
    from ollama_helper import ask_ollama

topic = input("Enter topic: ")

prompt = f"Generate 5 multiple choice questions on {topic} with four options and correct answers."

answer = ask_ollama(prompt)

print("\nMCQ Questions:\n", answer)

with open("mcq.txt", "w") as f:
    f.write(answer)
    24. Study Assistant
File: q24_study.py

from ollama_helper import ask_ollama

topic = input("Enter study topic: ")

prompt = f"Explain {topic} in simple words with important points and examples."

answer = ask_ollama(prompt)

print("\nStudy Assistant:\n", answer)

with open("study_notes.txt", "w") as f:
    f.write(answer)
    
    25. Flashcard Generator
File: q25_flashcard.py

    from ollama_helper import ask_ollama

topic = input("Enter topic: ")

prompt = f"Create 5 question and answer flashcards about {topic}."

answer = ask_ollama(prompt)

print("\nFlashcards:\n", answer)

with open("flashcards.txt", "w") as f:
    f.write(answer)

    26. Meeting Minutes Generator
File: q26_meeting.py
from ollama_helper import ask_ollama

discussion = input("Enter meeting details: ")

prompt = f"Generate meeting minutes with summary, decisions and action items:\n{discussion}"

answer = ask_ollama(prompt)

print("\nMeeting Minutes:\n", answer)

with open("meeting_minutes.txt", "w") as f:
    f.write(answer)
    27. Resume Analyzer
File: q27_resume.py
from ollama_helper import ask_ollama

resume = input("Enter resume details: ")

prompt = f"Analyze the resume and suggest improvements, skills and strengths:\n{resume}"

answer = ask_ollama(prompt)

print("\nResume Analysis:\n", answer)

with open("resume_analysis.txt", "w") as f:
    f.write(answer)
    28. College FAQ Chatbot
File: q28_college_faq.py
from ollama_helper import ask_ollama

print("WELCOME TO COLLEGE FAQ CHATBOT")

while True:
    question = input("\nAsk your question (exit to stop): ")

    if question.lower() == "exit":
        break

    prompt = f"Answer this college-related question. If information is unavailable, say so:\n{question}"

    answer = ask_ollama(prompt)
    29. Feedback Analyzer
File: q29_feedback.py
from ollama_helper import ask_ollama

feedback = input("Enter feedback: ")

prompt = f"Analyze the feedback and identify positive points, negative points and improvements:\n{feedback}"

answer = ask_ollama(prompt)

print("\nFeedback Analysis:\n", answer)

with open("feedback.txt", "w") as f:
    f.write(answer)

    print("\nChatbot:", answer)


    30. Email Assistant
File: q30_email.py
from ollama_helper import ask_ollama

email = input("Enter email message: ")

prompt = f"Act as an email assistant. Correct grammar and generate a professional email reply:\n{email}"

answer = ask_ollama(prompt)

print("\nGenerated Email:\n", answer)

with open("email_reply.txt", "w") as f:
    f.write(answer)

    
    
    
    
