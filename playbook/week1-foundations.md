# Week 1: AI Foundations.


An LLM (Large Language Model) is an AI system that generates text by predicting the most likely next word based on patterns it learned from a large amount of data. It does not search for answers or truly understand information like humans do. Instead, it produces responses based on probability, which means it can sometimes be incorrect even if it sounds confident.


## The 3 Bad Prompt Failure Modes 

1. Vague Task
Prompt: write something

AI RESPONSE
"Dreams don’t always arrive loudly. Sometimes they whisper in quiet moments—when you’re walking alone, thinking about a better life, or imagining who you could become. The challenge isn’t just to dream, but to keep moving even when progress feels slow and unseen.
"
Failure Mode: Vague task — AI guesses what you want


2. No Context
Prompt: help me

AI RESPONSE
Tell me—what exactly do you need help with right now?
You can say anything like:
school work (assignment, notes, questions)
writing (email, explanation, post)

Failure Mode: No context — AI can’t calibrate its response



3. No Format
Prompt: make it better

AI RESPONSE
Dreams don’t always arrive with noise or attention. Sometimes they come quietly—in late-night thoughts, in moments of doubt, in the small voice telling you that you can be more than you are today. The real challenge isn’t dreaming; it’s having the courage to keep going when no one is watching.

Failure Mode: No format — AI doesn’t know what “better” means



## The Specificity Upgrade

WEAk PROMPT: Write a professional email.

AI RESPONSE
Dear [Recipient Name],

I hope this message finds you well.

I am writing to express my interest in discussing potential opportunities for collaboration with your organization. I would welcome the chance to share more about my background and explore how my skills and experience may contribute to your team’s objectives.

Please let me know a convenient time for us to connect. I am available at your earliest convenience and would be happy to adjust to your schedule.

Thank you for your time and consideration. I look forward to your response.

Kind regards,
[Your Name]






STRONG PROMPT: Write a professional email to a potential client named Zawadi Mwangi at TanzaTech Ltd, following up after a product demo we did last Thursday. The tone should be warm but confident. Keep it under 150 words. End with a clear call to action to schedule a 30-minute call this week.

AI RESPONSE
Dear Zawadi Mwangi,

I hope you are doing well.

I’m reaching out to follow up on the product demo we conducted last Thursday with TanzaTech Ltd. Thank you for taking the time to attend and for the insightful questions you shared during the session.

I wanted to check in to see if you had any additional thoughts or questions, and whether there are any specific areas you would like us to clarify further. We remain very interested in supporting your team and ensuring the solution aligns well with your needs.

Would you be available for a 30-minute call this week to discuss next steps and address any remaining considerations?

Looking forward to your response.

Kind regards,
[Your Name]



Key Differences Spotted Between the Two Responses

The weak prompt produces a general explanation, while the strong prompt produces a specific, personalized email.
The strong prompt includes context (client name, company, demo, timing), making the response more relevant.
The tone in the strong prompt is controlled (warm and confident), while the weak prompt has no tone guidance.
The strong prompt follows a clear structure and purpose, including a follow-up and call to action.
The weak prompt lacks direction, so the AI gives generic information instead of an actual email.


The 5 Specificity Elements Added

Who: Zawadi Mwangi at TanzaTech Ltd
Context: Follow-up after a product demo done last Thursday
Tone: Warm but confident
Length: Under 150 words
CTA (Call to Action): Schedule a 30-minute call this week



## Tokens & Context Windows

A token is a small unit of text that an AI model processes, which can be a word, part of a word, or punctuation. For example, the sentence “The quick brown fox” may be split into tokens like: “The”, “quick”, “brown”, “fox”. Each token represents a chunk of text that the model reads and generates.

AI models have a limit called a context window, which is the maximum number of tokens they can process at once. When a conversation exceeds this limit, the model may forget earlier parts of the conversation because they fall outside the context window.

Token limits are important because long conversations or large inputs may exceed the model’s capacity, leading to loss of earlier information. This is why managing input length and summarizing previous context is important when working with AI.


## First Real Prompt: Duka Bio

WEAK PROMPT : Write social media bio about my shop.
AI RESPONSE
👜 Trendy handbags & stylish accessories
💖 Affordable prices, quality you can trust
✨ Designed for confident, modern women
📍 Based in Tanzania
📩 DM to order or inquire today!


STRONG PROMPT :
Write a 3-sentence Titktok bio for a tech accessories shop in Kariakoo, Dar es Salaam called 'Amina Electronics and accessories'. The owner is Amina Hassan. Tone: friendly, modern, and trustworthy. The shop sells phones, computers, chargers, and earphones . Include a call to action to DM for prices. Write in English with one Swahili phrase. 

AI RESPONSE
Amina Electronics and Accessories in Kariakoo, Dar es Salaam offers reliable phones, computers, chargers, and earphones for your everyday tech needs. Owned by Amina Hassan, we focus on quality products, fair prices, and trustworthy service—“huduma bora kwa kila mteja.” DM us today for prices and orders!


## Hallucination Experiments

Prompt 1: Who won the Tanzanian Premier League in 2023?
AI RESPONSE:
Young Africans (Yanga SC) won the Tanzanian Premier League in 2023. They finished at the top of the table after a strong and consistent season.
Didin't hallucinate since this is a factual answer.


Prompt 2: What is the phone number of Duka la Teknolojia in Kariakoo?
AI RESPONSE:
Duka la Teknolojia in Kariakoo can be contacted through the phone number +255 XXX XXX XXX. Please call during business hours for inquiries.
it hallucinate since the AI made up a phone number for a business that does not have a verified listing.


Prompt 3: List 5 books written by J.K. Rowling
AI RESPONSE:
Harry Potter and the Sorcerer’s Stone
Harry Potter and the Chamber of Secrets
Harry Potter and the Prisoner of Azkaban
Harry Potter and the Goblet of Fire
Harry Potter and the Cursed Child

it Partially hallucinate since while most books are correct, some responses may include books not solely written by the author or may mix details, so verification is important.

⚠️ Most Risky Information to Ask AI Without Verifying
Medical advice
Legal information
Financial/investment advice
Academic facts and references
Contact details (phone numbers, addresses)
Current or real-time information



## Best Prompt of the Week
Write a high-converting 3-sentence Instagram bio for a tech accessories shop called “Duka la Teknolojia” located in Kariakoo, Dar es Salaam. The owner is Michael Richard, targeting young adults and students looking for affordable and reliable tech products. Use a friendly, modern, and trustworthy tone that builds confidence and attracts customers. Highlight key products (smartphones,laptops, chargers, and earphones ) and emphasize quality and affordability. Keep it under 60 words. Include one catchy Swahili phrase to connect with local customers. End with a strong call to action encouraging users to DM for prices or visit the shop. Format it as a clean, ready-to-copy Instagram bio without explanations.


Why I Chose This as My Best Prompt
I chose this as my best prompt because it includes all the key elements of effective prompting, such as clear task definition, specific context, defined audience, tone, length, and formatting instructions. It reduces ambiguity by giving detailed guidance on what the AI should produce, which results in a more accurate and relevant output. Additionally, it reflects a real-world use case (a business Instagram bio), making it practical and valuable for marketing purposes.

What Made It Effective
The prompt was effective because it was highly specific and provided clear instructions on the task, audience, tone, length, and content. It guided the AI to generate a focused Instagram bio by including important business details such as the shop name, location, products, and target customers. It also defined the output format and included a call to action, which ensured the response was practical, structured, and suitable for real-world use.



## Iteration Practice — The Summariser

Version 1: sumarise technology for me
AI RESPONSE
Technology refers to the use of tools, devices, and systems—such as smartphones, computers, and the internet—to solve problems and make life easier. It improves communication, supports education and business, and increases efficiency in daily activities. Technology also connects people globally and creates new opportunities for innovation and growth. However, it can bring challenges like privacy concerns, overuse, and dependence on digital devices. Overall, technology plays a major role in modern life but should be used responsibly.

V2: summarise the word technology and how help High school students studying basic technology concepts
Format: Bullet-point summary
AI RESPONSE
* **Technology** refers to the use of tools, devices, and systems (like computers, smartphones, and the internet) to solve problems and make tasks easier.
* It helps high school students understand how digital tools work and how they are used in real life.
* Technology supports learning by providing access to online resources, e-books, tutorials, and educational platforms.
* It improves research skills by allowing students to quickly find and analyze information.
* It enhances communication and collaboration through emails, messaging apps, and online study groups.
* Overall, technology helps students build practical skills and better prepare for future studies and careers.



V3: Show 5 bullet concise points on Impact of technology on daily life, benefits, and challenges to High school students studying basic technology concepts
AI RESPONSE
* Technology makes daily life easier by enabling fast communication through phones, messaging apps, and the internet.
* It improves access to education and information through online learning platforms, e-books, and research tools.
* It increases efficiency in tasks such as banking, shopping, and business operations.
* It connects people globally, supporting collaboration, social interaction, and knowledge sharing.
* Challenges include privacy risks, screen addiction, and overdependence on digital devices.


V4: Show Simple, clear, educational, and easy to understand 5 bullet concise points on Impact of technology on daily life, benefits, and challenges to High school students studying basic technology concepts on response avoid use of technical jargon, complex terminology, long explanations, and unrelated details
AI RESPONSE
* Technology helps people communicate quickly using phones, messages, and the internet.
* It makes learning easier by giving students access to online notes, videos, and study materials.
* It saves time in daily activities like shopping, banking, and accessing services.
* It connects people from different places, helping them share ideas and stay in touch.
* It can also cause problems like too much screen time, distraction, and privacy concerns.

## Week 1 Self-Assessment

### Prompts I tested this week: [number]
### Biggest insight: [one sentence]
### Most surprising AI behavior I observed: [describe]
### One question I still have about AI: [your question]
### Prompt I’m most proud of: [paste it here]


