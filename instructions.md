# Senior Software Engineer Assignment

We're thrilled you're interested in joining SimPPL! This assignment is designed to give you a taste of the kind of engineering challenges we tackle.  You'll build a system for collecting social media data, with a focus on scalability and robust design. You will need to build a basic data collection platform to collect data from some fringe social networks within platform terms of service. 

## Platform Choices 
Some examples that may guide you in learning more about smaller platforms including some so-called fringe platforms (since there are existing data collection tools for these platforms already), in order of priority for the kinds of platforms we’d like to see you analyze. 

Note: Pick a minimum of one and a maximum of two platforms from which you will gather data, host your own system with search capabilities for the platform's data. Bonus points if you are able to include mobile-based platforms, present a set of inferences via graphs and analyses, and conduct multilingual, or multimodal analysis. We added links to platforms that you may not have heard of to make them easy for you to find.

1. Gab
2. Threads (Meta)
3. ShareChat
4. [Josh](https://myjosh.in)
5. 4chan
6. Telegram
7. Bitchute
8. Rumble
9. [Moj](https://mojapp.in/)
10. Mastodon
11. [VK](https://vk.com)
12. [Win Communities](https://communities.win), especially [Patriots](https://patriots.win)
13. Meta
14. Reddit

## Why do we care about this?

We have built tools for collecting and analyzing data from Reddit and Twitter including [Parrot](https://parrot.simppl.org) to study the sharing of news from certain unreliable Russian media providers. To ramp you up towards understanding how to go about extending such platforms, and to expand your understanding of the broader social media ecosystem, we would like you to construct a similar analysis to Parrot by studying other publicly accessible platforms listed above. We would like you to present an analysis of a broader range of viewpoints from different (apolitical / politically biased) groups. You may even pick a case study to present e.g. a relevant controversy, campaign, or civic event. 

In the long run, this research intends to accomplish the following objectives:

1. Track different popular trends to understand how public content is propagated on different social media platforms.
2. Identify posts containing misleading information with the use of claims verification mechanisms.
3. Analyze the trends across a large number of influential accounts over time in order to report on the influence of a narrative.

## Task Objectives

1. **Data Collection**: Develop a scraper that collects data from one of the listed social media platforms.  Your scraper should gather post content, engagement metrics (likes, shares, etc.), user information, and timestamps and should be able to collect data based on hashtags, keywords, news links, and user queries. Implementing multiple data collection methods will earn bonus points.
2. **System Design**: Create a system design (in words and with a diagram) that explains how your data collection solution can be scaled to handle a large volume of data and potentially multiple social media platforms *without being blocked by the platform within reasonable scale*. Consider cloud infrastructure, data storage, processing pipelines, and any APIs or services you would use.

Note: 
   a. You may use [Figma](https://figma.com) or [draw.io](https://draw.io) for the system design diagram but please commit it as a PNG or JPG image to your repository so we can access and evaluate it.
   
   b. Platforms block web scraping using HTML and [Beautifulsoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) quite easily so that will not be a great solution.

## Rubric for Evaluation

1. Functionality: Does the scraper function reliably, collect the required data, and store it in a specific location that we can access to verify the collected data?
2. Scalability: Is the system design well-thought-out and scalable? Does it address the potential challenges of handling large datasets and multiple platforms? Does the solution scale beyond just one-time searches (e.g. scraping HTML off of web pages may be easy to implement but will not scale to social media, because it may violate some of their terms and will immediately get flagged and blocked)?
3. Data Collection and Search: Is there a search functionality for data collection using news URLs, hashtags, keywords, or queries across the platform, made available through this solution?
4. Documentation: Is the code and system design modular, well-documented, and easy for a beginner to understand? Does your system diagram clearly illustrate the architecture of the entire data pipeline, from user queries to data storage? Does it show how queries are processed, the specific data collected, the transformation steps, and the storage solutions used? Additionally, does the diagram explain how the system handles concurrent requests and provide a high-level overview of your chosen cloud infrastructure and services, along with the rationale behind your choices? A clear and well-explained diagram demonstrating a scalable design is highly valued.

Bonus Points: 
1. Additional points will be awarded for mobile-based platforms with limited API documentation to collect data.
2. Design and build an interactive dashboard to analyze and visualize this data, uncovering patterns and insights about how specific links, hashtags, keywords, or topics are being shared and discussed.

## Instruction for the submission

These instructions outline how to use GitHub for this assignment. Please follow them carefully to ensure your work is properly submitted.

1. Fork the Repository:    
   - Go to the assignment repository provided by the instructor: [Insert Repository Link Here] 
   - Click the "Fork" button in the top right corner of the page. This creates a copy of the repository in your GitHub account. 
  
3. Clone Your Fork:
   - Go to your forked repository (it will be in your GitHub account).
   - Click the "Code" button (the green one) and copy the URL. This will be a git URL (ending in .git).
   - Open a terminal or Git Bash on your local machine.
   - Navigate to the directory where you want to work on the assignment using the cd command. For example: `cd /path/to/your/projects`.
   - Clone your forked repository using the following command: git clone <your_forked_repository_url> (Replace <your_forked_repository_url> with the URL you copied).
  
   This will download the repository to your local machine.

4. Develop Your Solution

   Work on your assignment within the cloned repository. Create your code files, visualizations, and any other required deliverables. Make sure to save your work regularly.

6. Commit Your Changes
   - After making changes, you need to "stage" them for commit. This tells Git which changes you want to include in the next snapshot.
   - Use the following command to stage all changes in the current directory:
      - To add all the files - git add. 
      - Or, if you want to stage-specific files - git add <file1> <file2> ...
   - Now, commit your staged changes with a descriptive message- git commit -m "Your commit message here" (Replace "Your commit message here" with a brief1 description of the changes you made.2 Be clear and concise!)
   - Push your commits back to your forked repository on GitHub- git push origin main (Or, if you're working on a branch other than main, replace main with your branch name. origin refers to the remote repository you cloned from). 
  
7. Please notify us of your submission by emailing simppl.collabs@gmail.com with the subject line "Submitting ML Engineer Assignment for SimPPL".

### Submission Requirements

Please ensure you include:

1. A detailed README file (with screenshots of your solution, a _hosted_ web platform).
2. A text-based explanation of your code and thought process underlying system design. 
3. Detailed documentation and a PNG or JPEG file of your system design.

Both of these last two make it easier for us to run your code and evaluate the assignment.

### Resources

1. [OSINT Tools](https://start.me/p/0Pqbdg/osint-500-tools)
2. [Colly](http://go-colly.org/)
3. [AppWorld](https://appworld.dev/)
4. [Scrapling](https://github.com/D4Vinci/Scrapling)
5. [Selenium](https://www.selenium.dev/)
6. [Puppeteer](https://pptr.dev/)
7. [DuckDB](https://github.com/duckdb/duckdb)
8. [Cloudfare Workers](https://workers.cloudflare.com/)
9. [Apache Superset](https://github.com/apache/superset)
10. [Terraform](https://www.hashicorp.com/en/products/terraform)

### Sample assignments from internship applicants

1. [Mojster](https://github.com/usyntest/mojster)
2. [YouTube Dashboard](https://github.com/DarshanJain-07/youtube_dashboard)


#### Note

Focus on the analysis you are presenting and the story you are telling us through it. A well-designed and scalable system is more important than a complex one with a ton of features. Consider using innovative technologies in a user-friendly manner to create unique features for your platform such as AI-generated summaries that are adaptable to the data a user searches for, using your platform.

Presentation matters! Make sure your submission is easy to understand. Create an intuitive and meaningful README file or a Wiki that can be used to review your solution. Host it so it is accessible by anyone. Ensure that you share a video demo even if it is hosted, so that users understand how to interpret the insights you present.

At SimPPL, we're building tools to analyze how information spreads on social media, especially from unreliable sources. Your work will help inform how to scale our analysis to a wider range of platforms and handle larger datasets. This is crucial for tracking trends, identifying misinformation, and understanding how narratives spread online.

We're excited to see your solution!

