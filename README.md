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
- **Languages:** (English).

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


%----------HEADING----------
\begin{document}
\begin{center}
{\Huge \scshape Muhammad Anis} \\ \vspace{3pt}
Backend Engineer (Java) \\ \vspace{3pt}
\small \faMapMarker*~ Islamabad, Pakistan ~|~ 
\faPhone~ +92-331-5942715 ~|~
\href{mailto:anis16734@gmail.com}{\faEnvelope~ anis16734@gmail.com} ~|~
\href{https://www.linkedin.com/in/muhammadaaanis/}{\faLinkedin~ linkedin.com/in/muhammadaaanis} ~|~
\href{https://github.com/muhammadanis418}{\faGithub~ github.com/muhammadanis418}
\end{center}

%-----------SUMMARY-----------
\section{Summary}
Backend engineer experienced in developing scalable RESTful APIs using Spring Boot. Strong in backend architecture, data performance, and problem solving. Currently expanding expertise in Cloud Deployment and CI/CD to deliver efficient, production-ready systems.

%-----------SKILLS-----------
\section{Technical Skills}
\resumeItemListStart
\resumeItem{Frameworks: Spring Boot, Spring MVC, Hibernate, JPA, J2EE}
\resumeItem{Databases: PostgreSQL, MongoDB, Redis}
\resumeItem{Languages: Java, SQL, JavaScript}
\resumeItem{Messaging: RabbitMQ, Kafka (basic)}
\resumeItem{Tools: Git, Maven, Swagger, Postman, Docker, IntelliJ IDEA, VS Code}
\resumeItem{Concepts: Microservices, RESTful APIs, OOP, Agile Development}
\resumeItemListEnd

%-----------EXPERIENCE-----------
\section{Professional Experience}
\resumeSubHeadingListStart

\resumeSubheading
{Ciklum}{Dec 2024 -- Present}
{Software Engineer}{Islamabad, Pakistan}
\resumeItemListStart
\resumeItem{Developing and refactoring Java-based vessel management modules for better performance and maintainability.}
% \resumeItem{Integrated Redis caching for fleet data to reduce DB calls and improve response time for multi-vessel datasets.}
\resumeItem{Integrated Redis caching for multi-vessel fleet data, cutting database load by 40 percent and reducing response times from seconds to milliseconds.}
\resumeItemListEnd

\resumeSubheading
{Target Technologies}{Jan 2024 -- Nov 2024}
{Backend Engineer (Java)}{Islamabad, Pakistan}
\resumeItemListStart
\resumeItem{Delivered features for Well \& Seismic data platform used by the Oman government.}
\resumeItem{Generated dynamic PDF reports using iTextPDF and optimized dashboard modules.}
\resumeItem{Configured Spring Cloud Eureka Server for service discovery in microservice architecture.}
\resumeItemListEnd

\resumeSubheading
{Rockville Technologies}{Jul 2022 -- Dec 2023}
{Junior Java Developer}{Islamabad, Pakistan}
\resumeItemListStart
\resumeItem{Enhanced APIs for Bajao music platform and contributed to Cellcard Music and UTunes services.}
\resumeItem{Built SMS handler pushing notifications via RabbitMQ to improve message delivery reliability.}
\resumeItemListEnd

\resumeSubheading
{Aksa SDS}{Dec 2021 -- Jun 2022}
{Java Intern}{Islamabad, Pakistan}
\resumeItemListStart
\resumeItem{Developed background automation tasks and CRUD APIs using Spring Boot.}
\resumeItem{Create an Address book application to demonstrate backend flow and data persistence.}
\resumeItemListEnd

\resumeSubHeadingListEnd

%-----------PROJECTS-----------


%-----------EDUCATION-----------
\section{Education}
\resumeSubHeadingListStart
\resumeSubheading
{COMSATS University}{Sep 2015 -- Jun 2019}
{B.Sc. Software Engineering}{}
\resumeSubHeadingListEnd

%-----------ACHIEVEMENTS-----------
\section{Achievements}
\resumeItemListStart
\resumeItem{Completed Web Engineering Bootcamp (Java) by Softoo Pvt. Ltd. (PASHA \& PSEB, 2022).}
\resumeItem{Received Benevolent Scholarship for academic excellence (2015–2019).}
\resumeItemListEnd

%-----------LANGUAGES-----------
\section{Languages}
\resumeItemListStart
\resumeItem{English (Intermediate Proficiency)}
\resumeItem{Urdu (Native Proficiency)}
\resumeItemListEnd

\end{document}
```
<!--
\section{Projects}
\resumeSubHeadingListStart
  \resumeProjectHeading
      {\textbf{Customer Churn Analysis} $|$ \emph{Python }}{March 2025 -- April 2025}
      \resumeItemListStart
        \resumeItem{\textbf{Analyzed behavior of 7,043 telecom customers} to identify churn patterns.}
        \resumeItem{Engineered new features including contract type buckets and tenure bands.}
        \resumeItem{Generated 11 visualizations to highlight churn-prone segments.}
        \resumeItem{Found 38\% of churned users were monthly-contract customers.}
      \resumeItemListEnd

  \resumeProjectHeading
      {\textbf{Sales Dashboard for Regional Performance} $|$ \emph{SQL, Power BI}}{February 2025 -- March 2025}
      \resumeItemListStart
        \resumeItem{Queried and joined 25,000+ rows of sales data using optimized SQL joins.}
        \resumeItem{Built KPIs and dynamic measures in Power BI.}
        \resumeItem{Designed multi-page dashboards with drill-down insights.}
        \resumeItem{Identified 14\% post-festival sales drop and recommended fixes.}
      \resumeItemListEnd
\resumeSubHeadingListEnd
-->

### Step 3: Compile Your Resume on Overleaf
Now we turn that code into a beautiful PDF.

- 🟢 Go to https://www.overleaf.com/.
- 🔵 Click "Register" and sign in with your Google account (it's free).
- 🟡 On your dashboard, click New Project > Blank Project.
- 🟣 Name your project (e.g., "My Resume").
- 🔴 You'll see a file named main.tex. Delete all the text inside it.
- 📋 Paste the full LaTeX code you got from ChatGPT into this empty main.tex file.
- ❇️ Click the green "Recompile" button (or press Ctrl+S).
### Step 4: Download Your Finished Resume!
- 🎉 On the right side of the screen, you will see your perfectly formatted, one-page resume.
- ⬇️ Click the "Download PDF" button (it looks like a down-arrow).
- That's it! You now have a professional, ATS-friendly resume ready to send to recruiters.

### 👍 Found this helpful?
If this video and guide helped you, please:

- Star this repository ⭐️
