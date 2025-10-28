# 🚀 The 4-Step Process

Here is the simple workflow we will follow to get resume ready.

---

## 🧩 Step 1: Choose Your Method (Prepare Your Data)

I cover **three ways to get started**. Pick the one that suits you best:

### 1️⃣ You Have an Existing Resume (PDF/DOCX) 📄
- Find your most recent resume (even if it's not ATS-friendly).  
- We will upload this file directly to ChatGPT and ask it to reformat it.

### 2️⃣ You Have an Updated LinkedIn Profile 🌐
- Go to your LinkedIn Profile.  
- Click the **“More”** button (below your name).  
- Click **“Save to PDF.”**  
- We will upload this PDF to ChatGPT.

### 3️⃣ You Are a Fresher (Starting from Scratch) ✍️
If you’re starting without a resume, no problem!  
Open a simple text file (like Notepad) and write down your details following this structure:

#### 🧾 Basic Structure
- **Profile Summary:** A short, powerful summary of who you are.  
- **Technical Skills:** (e.g., Programming, Tools, Databases).  
- **Projects:** Your most important projects with 2–3 bullet points each.  
- **Education:** Your degree, university, and graduation year.  
- **Achievements & Certifications:** (e.g., Hackathons, Google Certificates).  
- **Languages:** (e.g., English, Hindi).

> 💡 Tip: Once you have your data ready, we’ll move on to formatting it into a professional, ATS-friendly resume.

---

## ⚙️ Step 2: Generate the LaTeX Code with ChatGPT

This is the **most important step**. We will ask ChatGPT to write the LaTeX code for our resume.

1. Go to **ChatGPT (GPT-4 with file upload recommended).**  
2. Upload your file (from Method 1 or 2) **OR** paste your text (from Method 3).  
3. Use this exact prompt (only change `[Your Job Role]`):

> **Prompt to use:**
> ```
> Analyze this resume (file/text). I am applying for a [Your Job Role] role.  
> Please rewrite this as a strong, one-page, ATS-friendly resume.  
>
> You MUST use the exact LaTeX template I am providing below.  
> Generate the complete, ready-to-use LaTeX code for me.  
> Make sure all my information is filled in.
> ```

**CRITICAL:** Immediately after your prompt, paste the entire template below into the same message.

---

### 🧱 The One-Page LaTeX Template (Copy All of This)

#### For Backend Engineer Role Example

```latex
%-------------------------
% Resume in Latex
% Author: Muhammad Anis
%------------------------

\documentclass[letterpaper,11pt]{article}
\usepackage{latexsym}
\usepackage[empty]{fullpage}
\usepackage{titlesec}
\usepackage{marvosym}
\usepackage[usenames,dvipsnames]{color}
\usepackage{verbatim}
\usepackage{enumitem}
\usepackage[hidelinks]{hyperref}
\usepackage{fancyhdr}
\usepackage[english]{babel}
\usepackage{tabularx}
\usepackage{fontawesome5}
\usepackage{multicol}
\setlength{\multicolsep}{-3.0pt}
\setlength{\columnsep}{-1pt}
\input{glyphtounicode}

\pagestyle{fancy}
\fancyhf{}
\fancyfoot{}
\renewcommand{\headrulewidth}{0pt}
\renewcommand{\footrulewidth}{0pt}

\addtolength{\oddsidemargin}{-0.6in}
\addtolength{\evensidemargin}{-0.5in}
\addtolength{\textwidth}{1.19in}
\addtolength{\topmargin}{-.7in}
\addtolength{\textheight}{1.4in}

\urlstyle{same}
\raggedbottom
\raggedright
\setlength{\tabcolsep}{0in}

\titleformat{\section}{
  \vspace{-6pt}\scshape\raggedright\large\bfseries
}{}{0em}{}[\color{black}\titlerule \vspace{-5pt}]

\pdfgentounicode=1

\newcommand{\resumeItem}[1]{\item\small{{#1 \vspace{-2pt}}}}
\newcommand{\resumeSubheading}[4]{
  \vspace{-2pt}\item
    \begin{tabular*}{1.0\textwidth}[t]{l@{\extracolsep{\fill}}r}
      \textbf{#1} & \textbf{\small #2} \\
      \textit{\small#3} & \textit{\small #4} \\
    \end{tabular*}\vspace{-6pt}
}
\newcommand{\resumeProjectHeading}[2]{
    \item
    \begin{tabular*}{1.001\textwidth}{l@{\extracolsep{\fill}}r}
      \small#1 & \textbf{\small #2}\\
    \end{tabular*}\vspace{-6pt}
}
\newcommand{\resumeItemListStart}{\begin{itemize}}
\newcommand{\resumeItemListEnd}{\end{itemize}\vspace{-5pt}}
\newcommand{\resumeSubHeadingListStart}{\begin{itemize}[leftmargin=0.0in, label={}]}
\newcommand{\resumeSubHeadingListEnd}{\end{itemize}}

\begin{document}

%----------HEADING----------
\begin{center}
    {\Huge \scshape Vinay Kumar} \\ \vspace{4pt}
    \textbf{\Large \scshape Full Stack Developer} \\ \vspace{4pt}
    \small \faPhone\ +91-9919XXXXXX ~ 
    \href{mailto:advindiancoder@gmail.com}{\faEnvelope\ \underline{advindiancoder@gmail.com}} ~ 
    \href{https://www.linkedin.com/in/vinay-kumar860964/}{\faLinkedin\ \underline{linkedin.com/in/vinay-kumar860964}} 
\end{center}

%-----------SUMMARY-----------
\section{Summary}
Versatile and detail-oriented \textbf{Full Stack Developer} skilled in designing and deploying end-to-end web applications using Java, Spring Boot, React.js, and MySQL. Demonstrated expertise in RESTful API development, performance tuning, and scalable architecture. Passionate about clean code, open-source collaboration, and mentoring budding developers through technical content creation.

%-----------SKILLS-----------
\section{Skills}
\resumeItemListStart
  \resumeItem{\textbf{Frontend:} HTML5, CSS3, JavaScript (ES6+), React.js, Bootstrap, Tailwind CSS}
  \resumeItem{\textbf{Backend:} Java, Spring Boot, Hibernate, J2EE, JDBC, Servlets, REST API}
  \resumeItem{\textbf{Database:} MySQL, MongoDB}
  \resumeItem{\textbf{Tools \& Platforms:} Git, GitHub, Maven, Postman, Docker, IntelliJ IDEA, VS Code}
  \resumeItem{\textbf{Concepts:} OOP, MVC, Microservices, API Integration, Agile Development}
\resumeItemListEnd

%-----------EXPERIENCE-----------
\section{Experience}
\resumeSubHeadingListStart
  \resumeSubheading
    {Founder \& CEO — ADV SparkTech}{Aug 2023 -- Apr 2025}
    {Bengaluru, India}{}
    \resumeItemListStart
      \resumeItem{Developed and deployed multiple full-stack applications integrating REST APIs with MySQL databases.}
      \resumeItem{Led a 4-member developer team to deliver enterprise-grade projects with 35\% improved delivery speed.}
      \resumeItem{Mentored interns in Java and Spring Boot; improved project quality through peer code reviews.}
    \resumeItemListEnd

  \resumeSubheading
    {Full Stack Developer Intern — Inoglle (Part-Time)}{Jan 2024 -- Jul 2024}
    {Remote}{}
    \resumeItemListStart
      \resumeItem{Designed and implemented REST APIs in Spring Boot with JWT authentication and role-based access.}
      \resumeItem{Integrated React.js frontend with backend services, achieving 97\% uptime and responsive UX.}
      \resumeItem{Optimized MySQL schema resulting in 20\% faster query performance.}
    \resumeItemListEnd
\resumeSubHeadingListEnd

%-----------PROJECTS-----------
\section{Projects}
\resumeSubHeadingListStart
  \resumeProjectHeading
    {\textbf{E-Commerce Platform (Spring Boot + React.js + MySQL)}}{2024}
    \resumeItemListStart
      \resumeItem{Developed a full-stack online shopping system supporting user authentication, cart management, and secure payments.}
      \resumeItem{Optimized REST APIs for scalability, reducing latency by 25\%.}
    \resumeItemListEnd

  \resumeProjectHeading
    {\textbf{Student Management System (Java + JDBC + MySQL)}}{2023}
    \resumeItemListStart
      \resumeItem{Built CRUD-based application managing student data and grades with secure authentication.}
      \resumeItem{Applied normalization and indexing for faster query retrieval.}
    \resumeItemListEnd
\resumeSubHeadingListEnd

%-----------AWARDS & CERTIFICATIONS-----------
\section{Awards \& Certifications}
\resumeItemListStart
  \resumeItem{Microsoft Office 365 Productivity Suite (Advanced Level) — Naan Mudhalvan, 2022}
  \resumeItem{Top 5\% Global Designer on Canva — 2024}
  \resumeItem{Mock Technical Interview Score: 8.89/10 — 2024}
\resumeItemListEnd

%-----------EDUCATION-----------
\section{Education}
\resumeSubHeadingListStart
  \resumeSubheading
    {B.Tech in Information Technology}{Expected: 2025}
    {Dhaanish Ahmed College of Engineering (Anna University)}{CGPA: 8.2 / 10}
\resumeSubHeadingListEnd

\end{document}
