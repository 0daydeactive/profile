# OSINT -Level 1

```
Author: ABDULLAHI YUSUF Also known as 0daydeactice.
```

<details>

<summary>OSINT is a 3-level series that introduces Open-Source Intelligence (OSINT). It covers data collection, social media analysis, and investigative techniques, showing how publicly available information is used in cybersecurity and intelligence.</summary>



</details>

<figure><img src="https://miro.medium.com/v2/resize:fit:690/1*bcVtx3WThJIxosCCxZVpHQ@2x.jpeg" alt="" width="375"><figcaption></figcaption></figure>

> **Task 1 Prologue**

<details>

<summary>Welcome to the fascinating world of open-source intelligence. This course is designed to develop your skills from a total novice to an advanced investigator, guiding you step-by-step and level-by-level.</summary>



</details>

**Each level becomes more challenging, requiring the improvement of your search tactics, development of your analytical skills, and adoption of new investigative techniques. To make this more engaging, I will be providing you with CTF-style tasks at the end of each modu**le!

### 📌 Course Structure <a href="#ebb9" id="ebb9"></a>

#### 🛠 Level 1 – Foundations (Beginner) <a href="#bf53" id="bf53"></a>

💡 **The purpose of level 1 is to present basic capabilities for the collection and analysis of open-source information.**

#### 🔹 You will learn: <a href="#id-11a0" id="id-11a0"></a>

✅ **Google Dorking techniques to find hidden data on the web**

**✅ How to retrieve metadata from images and documents**

**✅ How to scrape social media footprints**

**✅ Using simple OSINT tools**

#### 🛠 Level 2 – Investigations (Intermediate) <a href="#id-13bd" id="id-13bd"></a>

◀️ **The overall objective of level 2 is to use your OSINT skills during real-life investigative situations that require thorough evaluation.**

#### 🔹 You will learn: <a href="#id-3916" id="id-3916"></a>

✅ **How to document your findings properly**

**✅ How to analyze data/information collected into reportable intelligence**

**✅ Provenance of open-source intelligence, including verification and cross-referencing**

**✅ How to run structured investigations**

#### 🛠 Level 3 – Advanced Techniques (Expert) <a href="#c8d4" id="c8d4"></a>

💡 **Unlike levels 1 and 2, level 3 is targeted towards anyone interested in high-level OSINT methodologies applied to cybersecurity, forensics, and intelligence domains.**

#### 🔹 You will learn: <a href="#e117" id="e117"></a>

✅ **OSINT tools for geolocation techniques**

✅ **Geospatial Intelligence (GEOINT)**

✅ **Personally Identifiable Behavior (PIB) & Operation Security (OPSec)**

✅ **The Berkeley Protocol**

#### 📌 **What to Expect in Level 1** <a href="#id-5501" id="id-5501"></a>

> **This introductory level offers five hands-on tasks aimed at building the foundation of your OSINT skills:**

1️⃣ **Google Dorking** – Use advanced search queries to uncover hidden information.

2️⃣ **Intro to OSINT** – Explore the fundamentals of OSINT investigations.

3️⃣ **Metadata Extraction** – Dig into files and images for data hidden in plain sight.

4️⃣ **The Footprint** – Detect user handles and tracks.

5️⃣ **OSINT Quick Quiz** – Test what you have learned!

**Each challenge will dive into a core OSINT technique, offering a practical exercise to apply what you’ve learned!**

🚀 **Your journey begins now. Let’s dive in.**

> **Task 2 Google Dorking Basics**

**Let’s begin learning!**

**This task will introduce you to Google Dorking and educate you on how to locate publicly available data ethically and apply your knowledge in a real-world scenario.**

#### What is Google Dorking? <a href="#id-954f" id="id-954f"></a>

<mark style="color:red;">**Google Dorking (Otherwise known as Google Hacking)**</mark> **is a search technique that uses advanced search operators to refine Google search results. It allows investigators, cybersecurity professionals, and researchers to uncover publicly available, but hard-to-find, data/information.**

**Many websites store PDFs, Excel Sheets, admin panels, and reports online. However, these files are not always linked on their main pages. Google automatically indexes many of these files, making them searchable if you know how to look for them.**

**On an important note, Google Dorking is a powerful tool that must be used ethically. It is legal when searching for publicly available data. On the other hand, using it to access restricted or unauthorized content violates the Terms of Service (ToS) and could be illegal.**

**Let’s go over some of the basic search operators:**

**site: – Used to limit results to a specific website.**

**inurl: – Used to find pages with a specific word in the URL.**

**intitle: – Utilized for searches for keywords in the page title.**

**intext: – Utilized to search for a keyword within the webpage content itself.**

**filetype: – Used to find a specific filetype(s) like DOCs, PDFs, XLSX, etc.**

**To refine your search results even more, we use specific key terms which include:**

**OR – Used to search for either of the words (Example.com OR Examples.com).**

**AND – Used to make sure that both (or more) words must be present (Alice AND Bob).**

**(-) The Minus Sign – Utilized to exclude word(s) from the results (Example.com -Press-release)**

**Let us take a look at this example task:**

**Here is an example scenario:**

<details>

<summary>“A major financial watchdog agency, the Consumer Financial Protection Bureau (CFPB), publishes annual financial reports detailing government expenditures and budgets. These reports are meant for public access, but they aren’t always easy to find. A whistleblower has informed us that the CFPB’s Financial Report for FY 2024 contains critical financial data that could affect upcoming government policies. However, for reasons unknown, the agency has not linked this document directly on its main website. It’s out there but hidden. Your job is to locate it using Google Dorking. We believe the document is still indexed by Google but buried within the agency’s digital archives.”</summary>



</details>

**Now that we know this, let’s handle this case!**

**Since we know it is a government entity, we know that the site uses a “.gov” extension and is released in a PDF.**

**Let’s try inputting site: .gov filetype: PDF in the search bar!**

**Hmm, it seems that we are getting .gov-only sites and the file types are indeed in PDF. However, we could not find the required document the reporter is looking for. We should refine our search to be even more specific!**

**Let’s try inputting site: .gov filetype: PDF “financial report” in the search bar instead!**

**Would you look at that? We found it! This is the financial report of the Consumer Financial Protection Bureau (CFBP) 2024.**

**Now, use the information that we have found to answer the questions below!**

<details>

<summary>Use the search (site: .gov filetype: pdf financial report intext: CFBP 2024) for extra assistance!</summary>



</details>

#### **Answer the questions below:** <a href="#c4b9" id="c4b9"></a>

> #### **What is the name of the Chief Financial Officer of the CFPB as mentioned in the PDF?**

&#x20;  **Janfar Gueye**

> #### What was the Total Fund Balance with Treasury in 2024?

&#x20;  **25,068,469**

> #### **What is the duration of the CFPB Supervisor Development Seminar?**

&#x20;       **3 days**

<figure><img src="https://miro.medium.com/v2/resize:fit:700/1*b7tTEG1_kCD6KibfBfYQRw@2x.jpeg" alt=""><figcaption><p>So now , we found the financial report of the – <a href="http://file.consumerfinance.gov">file.consumerfinance.gov</a></p></figcaption></figure>

<figure><img src="https://miro.medium.com/v2/resize:fit:700/1*SNOBAiHiRjeQahb9WUYn9g@2x.jpeg" alt=""><figcaption><p>Name of Chief Financial Officer of CCPB <strong>Jafnar Gueye</strong></p></figcaption></figure>

<figure><img src="https://miro.medium.com/v2/resize:fit:700/1*ddQeSGe9mux7SriNqowv6g@2x.jpeg" alt=""><figcaption><p>Fund Balance with Treasury 25068469</p></figcaption></figure>

<figure><img src="https://miro.medium.com/v2/resize:fit:700/1*JYZe92O5iS0gZtOot3qUjA@2x.jpeg" alt="" height="297" width="700"><figcaption><p>Duration of CFPB Supervisor Development Seminar is 3 days</p></figcaption></figure>

> #### **Task 3 Introduction to OSINT**

#### Your last task required you to use Google Dorking to track down a missing government report; That was just the beginning. <a href="#ce61" id="ce61"></a>

#### The real world is filled with information, some hidden in plain sight while others are buried within digital trails. Open-source intelligence (OSINT) is the skill of gathering, analyzing, and using publicly available data to solve investigations, uncover hidden truths, and track down individuals or organizations. <a href="#id-6f17" id="id-6f17"></a>

**So, what is OSINT?**

<mark style="color:$info;">**OSINT (Open-Source Intelligence)**</mark>**&#x20;refers to the collection and analysis of publicly available information to generate actionable insights. In the last exercise, we used a portion of OSINT; we utilized the usage of search engines to find a specific PDF file that relates to the scenario created for the sake of this training. So, what does OSINT consist of?**

**OSINT consists of:**

1. **Websites & Search Engines (Google, Bing, DuckDuckGo, etc.)**
2. &#x20;**Social Media Platforms (Twitter, LinkedIn, Facebook, etc.)**
3. &#x20;**Government Databases (FOIA records, court documents, etc.)**
4. &#x20;**Domain & IP Lookup Tools (Whois, Shodan, etc.)**
5. **Public Forums & Dark Web Resources and more!**

#### <mark style="color:yellow;">Who Uses OSINT?</mark>

**1.Cybersecurity Professionals use OSINT to assess digital footprints and security risks. Think of areas in cybersecurity like Threat Intelligence and Threat Hunting.**

**2. Law Enforcement & Investigators use OSINT to track criminals and locate missing persons.**

**3. Journalists & Researchers use OSINT to verify facts and expose misinformation.**

**4. Hackers, both ethical and unethical, & Threat Actors use OSINT to gather intelligence.**

**As a reminder, OSINT is powerful, but it must be used responsibly. Accessing publicly available data is legal, but attempting to bypass security measures or extract private information without consent crosses ethical and legal boundaries which makes us no different from the threat actors we fight.**

**OSINT-Related Organizations:**

<details>

<summary>I would like to take the opportunity to bring to your attention some organizations that are utilizing OSINT and strive to make a difference globally! While I can’t name every organization, I would like to name some who I have heard about and/or volunteered/worked with.</summary>



</details>

**Trace Labs:** [**https://www.tracelabs.org/**](https://www.tracelabs.org/)

**Kase Scenarios:** [**https://kasescenarios.com/**](https://kasescenarios.com/)

**OSMOSIS Institute:** [**https://osmosisinstitute.org/**](https://osmosisinstitute.org/)

**NCPTF:** [**https://ncptf.org/**](https://ncptf.org/)

**ClickSafe Intelligence:** [**https://clicksafeintelligence.com/**](https://clicksafeintelligence.com/)

**And the list goes on and on! For the investigators and professionals in this field, thank you from the bottom of our hearts!**

**Now, I leave you with your new task!**

<details>

<summary>“Intel Corporation has recently appointed Lip-Bu Tan as its new Chief Executive Officer (CEO). Investors and analysts are monitoring this change closely, and your task is to verify key details of his appointment using OSINT techniques. Our mission is to use advanced Google search operators to uncover specific information about Lip-Bu Tan’s appointment, previous role &#x26; board tenure”</summary>



</details>

**NOTE: This challenge follows legal and ethical OSINT practices. All information is publicly available through official company websites, press releases, and reputable news sources.**

🚨 <mark style="color:blue;">**DO NOT attempt to access private, restricted, or sensitive data. Stick to publicly available sources.**</mark>

**If you are having difficulty, refer back to the previous task!**

#### **Answer the questions below**

> #### **When was Lip-Bu Tan named the new Chief Executive Officer (CEO) of Intel Corporation?**

&#x20; **March 18, 2025**

> #### **Where did Lip-Bu Tan work before joining Intel Corporation?**

&#x20;  **Cadence Design Systems**

> #### **When was Lip-Bu Tan’s board tenure?**

&#x20;   **2022–2024**

<figure><img src="https://miro.medium.com/v2/resize:fit:700/1*ZxWkcP1uSSKLZkK0ApOj1Q@2x.jpeg" alt=""><figcaption><p>Use google hacking tips and get ans is march 18, 2025</p></figcaption></figure>

<figure><img src="https://miro.medium.com/v2/resize:fit:700/1*Hezq2Aeqa3xhgnt1qY3vaQ@2x.jpeg" alt=""><figcaption><p>Use google hacking tips and get ans is Cadence Design Systems</p></figcaption></figure>



<figure><img src="https://miro.medium.com/v2/resize:fit:700/1*vHrmrpm4Q2mQLzEXYOlTmw@2x.jpeg" alt=""><figcaption><p>Use google hacking and get the ans is 2022–2024 as you can see above.</p></figcaption></figure>

> **Task 4 Metadata Extraction**

<figure><img src="https://miro.medium.com/v2/resize:fit:474/1*Qft405fJKpKZw2yVU2lIXw@2x.jpeg" alt="" width="188"><figcaption><p>Download this image and then do analysis</p></figcaption></figure>

**Now that you are used to using advanced search queries, it is time to learn something new!**

**As an investigator, you will deal with a massive data load on a daily/weekly/monthly/yearly basis. Data can range from malicious files, error codes, false positives, etc. But, in the realm of OSINT, you might stumble upon Metadata.**

**Metadata is hidden data stored within files (PDFs, images, and documents) that can expose who created them, when, where, and with what device or software!**

**Some of the pieces of information we, as investigators, look at would be:**

**1- Creation Date**

**2- Modification Date**

**3-Author**

**4-Title**

**5-Subject**

**6-Software/Producer**

**6- Revision Number**

**7-Template Used**

**8- Company/Organization**

**9- Language Settings**

**10-GPS Coordinates**

**11-Make & Model**

**12-Resolution /Frame Rate**

**13-Device Software**

**14-Serial Number(s)**

**And many more pieces of information that can give us a general/specific idea of what we are looking at/dealing with.**

**We, investigators, use metadata to verify the sources, detect tampered documents (Or encrypted data), and inevitably track digital footprints that cybercriminals often forget to remove. That said, let me walk you through the process!**

Let us go over some tools that we, investigators, use:

<mark style="color:$danger;">**Tools Purpose**</mark>

<mark style="color:$success;">**Metadata2go**</mark> – Upload files to view metadata

<mark style="color:$success;">**Jeffrey’s Image Metadata Viewer**</mark> – Specialized for image metadata.

<mark style="color:$success;">**Diffchecker**</mark> – A data comparison tool that computes and shows the differences between the contents of files.

<mark style="color:$success;">**ExifTools**</mark> – Command-line metadata extraction tool (Advanced-Level) Sometimes, the software can reveal if a document was professionally created or edited by someone who wanted to hide something.

**Your mission:**

<details>

<summary>“A suspicious image has been anonymously uploaded to a public forum. While the content appears harmless, your goal is to analyze the metadata to uncover hidden details”</summary>



</details>

Use what you have learned to answer the three (3) questions below!

#### **Answer the questions below:**

> #### **Our investigators are looking for a tool to upload files to view metadata, which tool should they use?**

&#x20;  **Metadata2go**

> #### **Y/N: Metadata2go is a command-line metadata extraction tool.**

&#x20;  N

> #### **For Evidence(3), we got intel that the file does include an encrypted code that needs a key to open. The key seems to be “CODECOD”, what is the deciphered message?**

**THM(K@Y\_TO\_SUCCESS)**

<figure><img src="https://miro.medium.com/v2/resize:fit:700/1*oKq4NPrMSs7JgYHEFZpkfg@2x.jpeg" alt=""><figcaption><p>Download the file and then use metadata2go tool analys inage</p></figcaption></figure>

<figure><img src="https://miro.medium.com/v2/resize:fit:700/1*xYm4G8TuQ4Dr0OYMDR3mdw@2x.jpeg" alt=""><figcaption><p>You see description WPIO@A_HR_UIFGGGV</p></figcaption></figure>

<figure><img src="https://miro.medium.com/v2/resize:fit:700/1*J6iFZyCO3OLlvF-o1ho_Dw@2x.jpeg" alt="" height="310" width="700"><figcaption><p>Chose operator Vigenère Decode and put the key CODECOD. Put input VP(O@A HRUIGGGV) and then you see the ans is THM(K@Y_TO_SUCCESS)</p></figcaption></figure>

> **Task 5 Social Media Intelligence (SOCMINT)**

Time to explore how publicly available information from social media platforms can be gathered, cross-referenced, and used to build digital profiles, verify identities, or map networks, all ethically, legally, and powerfully!

#### **What is SOCMINT?** <a href="#id-3218" id="id-3218"></a>

**SOCMINT (Social Media Intelligence) is a branch of OSINT that focuses on collecting, analyzing, and interpreting information from social media platforms like:**

**. GitHub**

**. YouTube**

**. Reddit**

**. TikTok**

**. Facebook**

**. Twitter / X**

**. LinkedIn**

**. Instagram**

**. Even niche platforms like Soundcloud, Strava, Behance, etc.**

**Most investigations today, whether cybercrime, missing persons, threat intel, or fraud, have some trace on social media.**

**As we know, people can sometimes:**

**. Reuse usernames.**

**. Post photos with metadata.**

**. Cross-link platforms through bios or URLs.**

**. Reveal location clues, schedules, habits, and friends.**

**. Most importantly, forget that the internet never forgets.**

**SOCMINT gives you the eyes to see all of that, ethically. With the collected information, we can:**

**. Assist in locating missing people based on photos and online posts.**

**. Verify if a job applicant is lying on LinkedIn.**

**. Investigate criminal networks via social media followers.**

**. Map digital trails to connect sockpuppet accounts.**

**. Trace scammers by linking their bios across platforms.**

**As an investigator, you will follow a set of principles when using SOCMINT. Some of these core principles include:**

**Everything Must Be Public**

Never engage, log in, friend-request, or scrape private data. OSINT is ethical intelligence, not intrusion.

**Cross-Platform Analysis is King**

A Twitter handle leads to a GitHub: A GitHub leads to a LinkedIn. LinkedIn mentions a university. That university has a photo of a team. Now, you have a name.

**Reused Usernames Are Gold**

People are lazy : Most would reuse the same handle across multiple sites. Our job, as investigators, would be to find that repetition and validate the connection.

**Context Over Data**

Knowing someone posted on Instagram is fine. However, knowing they posted a vacation photo in a specific country at a specific time, while claiming they weren’t at said location, is intelligence.

Always remember, as Investigators, we also follow ethics when it comes to SOCMINT due to its power, meaning we handle that power with care. Do NOT Dox, Leak, Manipulate, or Intimidate. We are protectors of truth, not stalkers or threat actors. We work for what is right.

Now, let us look at some tools that we could use in a SOCMINT Investigation:

**Tool Purpose**

WhatsMyName – Find where a username exists across hundreds of platforms.

Namechk / Namecheckup – Verify username usage.

Google Dorking – Search specific platforms using keywords and operators.

Reverse Image Search – Match profile pictures across platforms.

**Answer the questions below**

> #### **Complete the following: The Internet**

&#x20;   **Never Forgets**

> #### **Our Investigators have found a username but are not sure if it is being used or not. Which tool would you suggest for the investigators to use?**

&#x20;  **Namecheckup**

> #### **A branch of OSINT that focuses on collecting, analyzing, and interpreting information from social media platforms is called…?**

&#x20; **SOCMINT**

> #### **Y/N: Jack plans to use SOCMINT to intimidate his friend. This is an example of ethical behavior.**

&#x20;     **N**

> #### **Task 6 OSINT Fusion**

<figure><img src="https://miro.medium.com/v2/resize:fit:700/1*PDT5EgxffcV4u0VxYIhqPw@2x.jpeg" alt="" width="375"><figcaption><p>Download this image and then do it analysis metadata</p></figcaption></figure>

**I leave you now with the final quest of Level 1 – OSINT**

<details>

<summary>“You receive an anonymous tip. No message. No explanation. Just a single image attached to a throwaway email account. The image is innocuous, just a professional-looking stock-style photo. At first glance, it looks like it could’ve been pulled from any business presentation. But something feels off. There’s no watermark. No branding. No source. Just a generic filename: Evidence(4). You decide to pull the metadata. Suddenly, things change. Someone’s name appears in the Artist field. Not a random name, a real person!”</summary>



</details>

**From here on, there are no step-by-step instructions. You’ll have to think like an investigator. No one’s going to tell you what the name means. You won’t be told who they are, where they work, or why the image was sent.**

🚨 <mark style="color:$danger;">**DO NOT attempt to access private, restricted, or sensitive data. Stick to publicly available sources.**</mark>

**Answer the questions below**

> #### **What is the name of the Artist that sent the image?**

&#x20; **Christina Lekati**

> #### **We have found that the user has a Twitter / X account. What is their handle?**

**@ChristinaLekati**

> #### **Looks like that image has a secret cipher that is encrypted, and our investigators need your help to decipher it.**

**THMC@ngratulations!}**

First download the image file and then analysis metadate of the image.

Use the tool&#x20;

<figure><img src="https://miro.medium.com/v2/resize:fit:700/1*oKq4NPrMSs7JgYHEFZpkfg@2x.jpeg" alt=""><figcaption><p>Metadata2Go</p></figcaption></figure>

<figure><img src="https://miro.medium.com/v2/resize:fit:700/1*YiFl0TCcIu16bCoCVAfVWQ@2x.jpeg" alt=""><figcaption><p>As you can see the artist name of Chriatinan Lekati</p></figcaption></figure>

<figure><img src="https://miro.medium.com/v2/resize:fit:679/1*051iSSO-qvZb83o-whfx3w@2x.jpeg" alt=""><figcaption><p>@ChristinaLekati</p></figcaption></figure>

<figure><img src="https://miro.medium.com/v2/resize:fit:700/1*A_9ZERH9pL_WY8Jgfgvuzw@2x.jpeg" alt=""><figcaption><p>Take and analys this comment its look like dcode info QEJ(Z@kdoxqr1xaflkp!]</p></figcaption></figure>

<figure><img src="https://miro.medium.com/v2/resize:fit:700/1*sfQNGKPN1tsJtMU14K3HEA@2x.jpeg" alt=""><figcaption><p>Use the cyberchef chose operator Caesar recipe ROT13 and chose 29 amount input QEJ(Z@kdoxqr1xaflkp!] and then you will see ans is THMC@ngratulations!}</p></figcaption></figure>

Finish the game.👏🏼

> **Task 7 Epilogue**

> **You started with a single image, a few clues, and a lot of uncertainty, but you kept digging, kept thinking, and proved that with the right mindset and ethics, even a small trail can lead to real answers. You respected the boundaries, uncovered what was hidden, and saw OSINT not as a shortcut, but as a responsibility. You didn’t just finish Level 1. You rose to it!**

Level 2 won’t hold your hand. But now… it won’t have to.

Here’s Room 2's link: [https://tryhackme.com/jr/osintledit2](https://tryhackme.com/jr/osintledit2)



<figure><img src="https://miro.medium.com/v2/resize:fit:700/1*nL_FDGke4wID3gozs8LLCw@2x.jpeg" alt=""><figcaption></figcaption></figure>
