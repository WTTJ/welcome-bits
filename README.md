# Welcome-bits

![Logo](logo_yellow_WTTJ.jpg)

[![Generic badge](https://img.shields.io/badge/Type-Newsletter-red)](https://medium.com/wttj-tech)
[![Generic badge](https://img.shields.io/badge/Frequency-Biweekly-blue)](https://medium.com/wttj-tech)
[![Generic badge](https://img.shields.io/badge/Open%20tech%20positions-3-green)](https://www.welcometothejungle.com/en/companies/wttj/jobs) 
[![Generic badge](https://img.shields.io/badge/Engineering%20blog%20articles-6-yellow)](https://medium.com/wttj-tech) 


**Welcome, dear \<reader>!**

**Every two weeks, we, the engineering team at Welcome to the Jungle, will share news about our tech products, as well as details about the technical topics we’ve been working on. Our newsletter, called Welcome Bits, will also include a curated list of the most interesting links we’ve found out there on the wild wild web.**

<details>
<summary>What is Welcome to the Jungle?</summary>
<p>

<a href="https://www.welcometothejungle.com/en">Welcome to the Jungle</a> is building the new experience at work. We use content and technology to transform every step of the employee experience, to help companies offer a better, more human experience in the workplace.</p>
</details>

<details>
<summary>Why we decided to create Welcome Bits</summary>
<p>
  
Learning and sharing knowledge is part of the engineering team’s DNA. For example, since Welcome to the Jungle launched, sessions called Jungle Labs have been organized each month so that developers in the team can spend one day away from their daily tasks to learn new stuff, grow technically, and share it all with the rest of the team (which is not always an easy exercise for the shyest among us).

So it seemed obvious to us that we should extend this learning and sharing experience to the outside world—meaning you, dear readers. And we hope you will enjoy reading about what we’ve discovered as much as we enjoy writing about it!</p>
</details>

<details>
<summary>The engineering team behind Welcome Bits</summary>
<p>
  
The team is currently made up of 14 developers, but we’re part of a bigger team called (no prizes for guessing) “the tech team,” which also encompasses product, data, design and QA people.

Welcome to the Jungle is based in Paris, France, but 65% of us are working in full remote mode, which means that some of us can code while enjoying a beautiful view of the mountains or ocean.

The engineering team is composed of back-end, full-stack, and front-end developers, as well as one DevOps engineer and one head of engineering. We are working with Elixir, Ruby, and React JS, among other technologies (you can check <a href="https://www.welcometothejungle.com/fr/companies/wttj/tech">our full stack</a> for more details).

If you want to know more about our team, and the tech team in general, take a look at <a href="https://youtu.be/9QAV5r-sFhI">the filmed interview with Kevin</a>, our beloved CTO.</p>
</details>

*This newsletter is a new thing for us, so your suggestions, questions, and comments are more than welcome! Just send us an issue or pull request.*

# Welcome Bits #4

# Archives

<details>
  
<summary>Welcome Bits #3</summary>

# Welcome Bits #3

## Bits of learning

“SQL is not that CRUD”

> We recently discovered a new function on PostgreSQL that allowed us to solve an issue we were having a hard time with. It’s the LAG function, which allows access to the data of the previous row, or the row before the previous row, and so on. Not sounding all that useful, right? But it really was! We were getting some duplicate entries on our database for movements between columns in a Trello-like board that allows recruiters to change the status of applicants. It wasn’t possible to use the “created at” data, as the duplicates were not created at the same date and time. But thanks to the LAG function, we were able to identify the movements that had the same previous movements, which allowed us to spot the duplicates. Who knows which unknown PostgreSQL function could help us fix our next issue?

*Bastien, back-end developer*

## Bits of curation

1. [Le refactoring le plus difficile de ma carrière (FR)](https://www.youtube.com/watch?v=TiRoge93H0o)

> Coding can become irrelevant when it starts affecting your health. In this talk, Jérôme Petazzoni shares his experience of suffering burnout. It’s a good reminder for all engineers that coding, and work in general, isn’t everything in life, no matter how passionate you are about it. (English subtitles are available on YouTube for non-French speakers—click on settings, then subtitles, then choose auto-translate.)

*Shawarma, head of engineering*

2. [New AI-Based Image Auto-Crop Algorithm Sticks to the Subject](https://cloudinary.com/blog/new_ai_based_image_auto_crop_algorithm_sticks_to_the_subject)

> A promising SaaS tool from Cloudinary that auto-crops images. We are currently looking for a way to manage image cropping for a feature that will alternate portrait and landscape images in one of our products. The Cloudinary solution is definitely one that we plan to have a closer look at and we will share our feedback in the newsletter, so stay tuned!

*Bastien, back-end developer*

3. [Fast Elixir](https://github.com/devonestes/fast-elixir)

> When it comes to performance, it’s always nice to have someone else doing the dirty work for you and benchmarking all the methods to see which is fastest. Well, here is the benchmarking tool for Elixir!

*Shawarma, head of engineering*

4. [CodeTour](https://github.com/microsoft/codetour)

> With 70 percent of our engineering team working fully remotely, we are currently looking for ways to improve the onboarding process of our developers. It looks like this Visual Studio Code extension could be something that will help us—and newcomers—by allowing us to create a guided tour of our main codebases!

*Samuel, back-end developer*

5. [Signs of triviality](https://www.netmeister.org/blog/email.html)

> Email validation at its finest! This is a good link to bookmark whenever you need to double-check that you have defined the right rules to apply when validating an email address that someone has entered on a form.

*Shawarma, head of engineering*

## Bits of exploration

### Project management with Jira (and Jira only)

At WTTJ, the tech teams are currently using both Trello and Jira as project management tools. Jira is used by other teams to report issues and request new features, while Trello is used by the tech teams to manage prioritization and follow up on these issues and features. So, yes, we pay both licenses. And yes, we manually import tickets from Jira to Trello every day.

But some of us are true Jira believers. We were convinced that Jira alone could fit our needs and even help us to improve our monitoring (which is quite basic in Trello at the moment). So we built a board in Jira and compared it to Trello to make our point. An important thing to note is that we chose [team-managed projects](https://support.atlassian.com/jira-software-cloud/docs/get-started-with-team-managed-projects/), as they offer more flexibility and are easier to manage than company-managed projects.

Here are the results: the strengths and limitations of Jira compared to Trello.

#### Strengths
- Jira’s features are the same as 90 percent of Trello’s features
- Epics can be managed without add-ons or workarounds
- It’s easy to get an overview of the project and provide visibility of the road map for the team
- It’s possible to manage sub-tasks, which are easier to manage than comments in Trello
- It’s possible to manage your backlog outside the board, which makes the board clearer and easier to read, and helps you to focus on what needs to be done first
- It provides access to the history of releases, independently of the board
- Several metrics and charts are available
- You are able to flag a ticket in a board
- It is easy to filter your board by epic, label, or assignee

#### Limitations
- It’s not possible to manage multiple assignees under one ticket
- Tags cannot be colored

So, as you have probably guessed, Jira won. After the presentation, three tech teams decided to migrate their projects to Jira. But this came with two conditions: First, the project needs to be mature enough. And second, we advise you to choose team-managed projects, as it allows your team to be autonomous when it comes to configuration.

## Bits of good vibes

Stéphane, our full-stack lead developer, contributed to [the latest release of Bamboo](https://github.com/thoughtbot/bamboo/pull/591), an open-source project that allows developers to use emails for Elixir. He worked on adding the ability to define interceptors for a given mailer, which can either be used to prevent emails from going out or to modify email data such as subject in a single place. Giving back to the open-source community is something that is very important to us and we definitely want to be able to contribute more in the future.

## Bits of jobs

There are currently 3 open positions in the engineering team:

[Engineering manager](https://www.welcometothejungle.com/en/companies/wttj/jobs/engineering-manager_paris)

[Full-Stack developer (Elixir, Ruby, React JS)](https://www.welcometothejungle.com/en/companies/wttj/jobs/full-stack-developer-ruby-elixir-react-js_paris)

[Back-end developer (Elixir, Ruby)](https://www.welcometothejungle.com/en/companies/wttj/jobs/backend-developer-ruby-elixir_paris_WTTJ_9MP4PxM)

If you have any questions about the positions, send us an issue or pull request!

Thanks for reading. As we’ve said, please don’t hesitate to open an issue or pull request for any questions or comments you might have about the newsletter or one of the job vacancies. We will answer you as soon as we can.
  
</details>

<details>
  
<summary>Welcome Bits #2</summary>
  
# Welcome Bits #2

## Bits of learning

"Be aware of how your users use your site"

> We noticed recently that we were getting a significant number of errors logged to Sentry, where we log all our front-end errors, with `SecurityError: Blocked a frame with origin “https://www.welcometothejungle.com” from accessing a cross-origin frame.`. Although Sentry is great at giving stacktraces including basic user interactions, we didn’t have much more to go on. After a bit of digging we found that it only surfaced in the Facebook in-app browser when users were trying to log in via LinkedIn. Our LinkedIn login implementation opened a popup window (as many sites do) with the LinkedIn login page so as not to disturb the user’s flow. Unfortunately, you can’t open popups in the Facebook browser or other apps that use an iOS WebView meaning anyone that opened a link in Facebook to one of our articles or job listings and then tried to log in ended up with a blank page and nowhere to go. Mildly frustrating to say the least. We’ve since changed the user flow so login/signup all happens in the same window. It’s slightly disruptive to the user experience — but much less disruptive than a blank page.

*Robert, full-stack developer*

## Bits of curation

1. [Before You memo()](https://overreacted.io/before-you-memo/) 

> A useful article by Dan Abramov that details two different techniques you can use in React instead of the memo() function. We’ve tried them both at WTTJ and they really helped to optimize performance.

*Mick, front-end developer*


2. [Strong Migrations](https://github.com/ankane/strong_migrations) 

> An interesting tool to use with projects, this detects issues during database migrations and is useful for the good practices its readme contains. Some serious issues we’ve encountered in the past would definitely have been avoided if we’d had this tool!

*Clément, back-end developer*


3. [Odyssey Design System](https://odyssey.okta.design)

> Odyssey is a new open-source project from Okta that provides users with a design system. Its UI includes lots of components related to sign-in and sign-up, as you would expect given what Okta’s business is, and there’s a strong focus on accessibility.

*Shawarma, head of engineering*


4. [The fire at OVH](https://twitter.com/olesovhcom/status/1369478732247932929?s=19)

> Millions of websites in France have been disrupted by the fire that broke out at OVH’s Strasbourg data center on March 10. It was a terrible event that should remind engineering teams everywhere how important it is to be prepared for the worst happening.

*Stéphane, full-stack lead developer*


5. [Flowchart.fun](https://flowchart.fun/ )

> Flowchart.fun is a really simple open-source tool for creating flowcharts from text and exporting them in various formats.

*Shawarma, head of engineering*

## Bits of good vibes

On March 17, our full-stack lead developer Stéphane became the proud father of Peio. Congratulations, Stéphane!

## Bits of jobs
There are currently 3 open positions in the engineering team:

[Engineering manager](https://www.welcometothejungle.com/en/companies/wttj/jobs/engineering-manager_paris)

[Full-Stack developer (Elixir, Ruby, React JS)](https://www.welcometothejungle.com/en/companies/wttj/jobs/full-stack-developer-ruby-elixir-react-js_paris)

[Back-end developer (Elixir, Ruby)](https://www.welcometothejungle.com/en/companies/wttj/jobs/backend-developer-ruby-elixir_paris_WTTJ_9MP4PxM)

If you have any questions about the positions, send us an issue or pull request!

Thanks for reading. As we’ve said, please don’t hesitate to open an issue or pull request for any questions or comments you might have about the newsletter or one of the job vacancies. We will answer you as soon as we can.

</details>

<details>
  
<summary>Welcome Bits #1</summary>

# Welcome Bits #1

## Bits of learning

"Optimizing your database the right way is never a waste of time"

> Over the past couple of weeks, we have been experiencing 40-plus million IOPS on some of our databases. Our first instinct was to check if any microservice was responsible for the high throughput, then we investigated AWS replicas, and finally we went after all the releases made in the past 6 months to look for any breaking change. But the answer to our performance issues was not there. So we started to look closer at the databases. We identified a lack of optimization and relevant indexes, and started to log slow queries and use pghero. After a few optimizations, we managed to halve the IOPS on our main database!

*Thomas, head of engineering*

## Bits of curation

1. [Pomerium](https://github.com/pomerium/pomerium) 

> A promising tool that could help us install a VPN to access our preproduction environment. Currently, we have to use multiple logins and passwords to access it, which is painful, and since some of my teammates have dynamic public IPs, we can’t filter on the IPs either. Pomerium seems more comprehensive than OpenVPN, which requires you to install additional tools to be able to manage identity aspects and policy access, and it has a Kubernetes API proxy.

*Charles, DevOps, security and back-end engineer*


2. [The styled-components happy path](https://www.joshwcomeau.com/css/styled-components/) 

> An article by Josh Comeau about the best practices for styled-components. I really like his blog posts about React and CSS because they are good quality, simple, and interactive. This one details the different ways you can lighten and simplify CSS files thanks to CSS variables and a single source of styles.

*François, front-end developer*


3. [Crypto-mining attack in my GitHub actions through Pull Request](https://dev.to/thibaultduponchelle/the-github-action-mining-attack-through-pull-request-2lmc)

> Unfortunately, attacks carried out on GitHub purely for personal benefit, like the one detailed in this article, and spam pull requests seem to be becoming more and more frequent. In addition to being contrary to open-source philosophy, this behavior also increases open-source maintainers’ fatigue, which can end up leading to burn-out. This is a real issue!

*Maxime, back-end developer*


4. [Numerical Elixir and Elixir XLA bindings for CPU/GPU/TPU](https://github.com/elixir-nx/nx)

> A very interesting first step to opening the Elixir language to machine learning and scientific calculations in a project led by José Valim himself and Sean Moriarity.

*Stéphane, full-stack lead developer*


5. [A performance dashboard for Postgres](https://github.com/ankane/pghero)

> We started using Pghero at the beginning of the year because we were encountering performance issues with some of our PostgreSQL databases. This library is great because it suggests indexes based on our queries and helps us to detect index overrides. It’s been really helpful!

*Sébastien, full-stack developer*


## Bits of exploration

### Visual testing using the Cypress plugin

The team has recently spent some time exploring visual testing, as we would like to implement it on the [Welcome UI](https://github.com/WTTJ/welcome-ui) design system. More specifically, we would like to be able to visually test the displayed components on the Welcome UI documentation, knowing that components can occur on different documentation pages.

We chose to test the [Cypress plugin](https://docs.cypress.io/guides/tooling/visual-testing.html#Functional-vs-visual-testing), which allows us to automatize the visual tests. 

Here is our condensed feedback about the Cypress plugin:

#### Strengths
- Free of charge
- Easy implementation
- Unit snapshots of components
- Web browsers and screen-resolution sensitive

#### Limitations
- Too sensitive: 
Comparison is done pixel by pixel, so the results are sometimes random. A threshold could be implemented to reduce the sensibility, but it could hide true anomalies.
- Limited debugging:
Differential snapshots are useful to indicate that there is an issue, but they are not clear enough to help with the analysis of the difference.

#### A concrete example with the breadcrumb component
- A visual test is executed for each line of the table, followed by the application design being modified:

![Screenshot](screenshot_test_cypress_plugin.png)

- Here is a snapshot of when a difference in the text of the breadcrumb component is found:

![Snapshot](snapshot_cypress_plugin_diff.png)

### API documentation using [GitBook](https://www.gitbook.com)

The team is currently searching for the most efficient way to create API documentation and has been putting GitBook through its paces to see if it is the answer.

#### Strengths
- Git-like versioning of the API
- Global documentation (API and tech documents, app setup, knowledge, and so on)
- Nice UI
- Easy to set up

#### Limitations
- A lot of small UI/UX bugs
- We didn’t find a way to set up a base_url for all the endpoints

#### The GitBook web UI

![Screenshot](GitBook_web_UI.png)

## Bits of good vibes

Our open-source customizable design system with React styled-components, styled-system and reakit, called [Welcome UI](https://github.com/WTTJ/welcome-ui), just reached 253 stars on GitHub! Don’t hold back from using it and/or contributing.

## Bits of jobs

There are currently 4 open positions in the engineering team:

[Engineering manager](https://www.welcometothejungle.com/en/companies/wttj/jobs/engineering-manager_paris)

[Full-Stack developer (Elixir, Ruby, React JS)](https://www.welcometothejungle.com/en/companies/wttj/jobs/full-stack-developer-ruby-elixir-react-js_paris)

[Back-end developer (Elixir, Ruby)](https://www.welcometothejungle.com/en/companies/wttj/jobs/backend-developer-ruby-elixir_paris_WTTJ_9MP4PxM)

[Front-end developer (React JS, CSS-in-JS)](https://www.welcometothejungle.com/en/companies/wttj/jobs/frontend-developer-react-js-css-in-js_paris)

If you have any questions about the positions, send us an issue or pull request!

Thanks for reading. As we’ve said, please don’t hesitate to open an issue or pull request for any questions or comments you might have about the newsletter or one of the job vacancies. We will answer you as soon as we can.

</details>
