# Welcome-bits WIP

## What is Welcome to the Jungle
[Welcome to the Jungle](https://www.welcometothejungle.com/fr) is a company creating the new experience at work. We use content and technology to transform every step of the employee experience to help companies offer a better, more human experience in the workplace.

## Why we decided to create Welcome Bits
Learning and sharing knowledge is part of the engineering team DNA. Since the beginning, Jungle Labs sessions are for instance organized each month so that developers in the team can spend a day away from their daily tasks to learn new stuff, grow technically, and share it with the rest of the team (which is not always an easy exercice for the shyest people among us).

So it seemed part of a continuing process to extend this learning and sharing experience to the outside world, meaning you, dear readers. And we hope you will enjoy reading it as much as we enjoyed writing it!

## What you will find in Welcome Bits
Every week, we will share news about our tech products as well as details about the technical topics we've been working on. The newsletter will also include a curated list of the more interesting links we found out there in the wild wild web.

This newsletter is quite new, so your suggestions, questions and comments are more than welcome! Send us an issue or a pull request to do so.

## The engineering team behind Welcome Bits
We are currently 14 developers in the engineering team itself, which is part of a bigger team called (what a surprise) "the tech team" where there are also product, data, design and QA people.

There are unfortunately only men right now in the engineering team, but as diversity is a value dear to our heart, our tech recruiter Xavier is working hard to hire women. If you are a woman who code, please check [our current opened positions](https://www.welcometothejungle.com/fr/companies/wttj/jobs) and apply if you are interested!

The company is based in Paris, France, but 65% of us are working in full remote mode, which means that some of us can code while enjoying a beautiful view on the mountains or the ocean.

The team is composed of back-end, full-stack and front-end developers, as well as one devOps engineer and one head of engineering. We are working with Elixir, Ruby and React JS among others (you can check [our full stack](https://www.welcometothejungle.com/fr/companies/wttj/tech) for more details).

If you want to know more about our team and the tech team in general, take a look at [the filmed interview of Kevin](https://youtu.be/9QAV5r-sFhI), our beloved CTO.

# 11th, February 2021

## Learning of the week

*"Optimizing your database the right way is never a waste of time"*

The last couple of weeks, we have been experiencing 40+ millions IOPS in some of our databases. Our first instinct was to check if any microservice was responsible for the high throughput, then we investigated AWS replicas and finally we went after all the releases that were made in the last 6 months to look for any breaking change. But the answer to our performance issues was not there... So we started to look closer at the databases. We identified a lack of optimisation and relevant indexes, and started to log slow queries and implement [pghero](https://github.com/ankane/pghero). After a few optimizations, we managed to divide by two our IOPS on our main database!

*By Thomas, head of engineering*

## 5 links that are worth checking out

## Good vibes

Our open-source customizable design system with react styled-components, styled-system and reakit, named [Welcome UI](https://github.com/WTTJ/welcome-ui), just reached 248 stars on GitHub! Don't hesitate to use it and/or contribute.

## We want you!

There are currently 5 positions opened in the engineering team:

[Engineering manager](https://www.welcometothejungle.com/en/companies/wttj/jobs/engineering-manager_paris)

[DevOps engineer](https://www.welcometothejungle.com/en/companies/wttj/jobs/devops-engineer_paris)

[Full Stack developer (Elixir, Ruby, React JS)](https://www.welcometothejungle.com/en/companies/wttj/jobs/full-stack-developer-ruby-elixir-react-js_paris)

[Back-end developer (Elixir, Ruby)](https://www.welcometothejungle.com/en/companies/wttj/jobs/backend-developer-ruby-elixir_paris_WTTJ_9MP4PxM)

[Front-end developer (React JS, CSS-in-JS)](https://www.welcometothejungle.com/en/companies/wttj/jobs/frontend-developer-react-js-css-in-js_paris)

If you have any question about the positions, send us an issue or a pull request!


Thanks for reading us. Don't hesitate to open an issue or a pull request for any question or comment you may have about the newsletter or one of the opened position. We will answer you as soon as we can. See you next week!