# Welcome-bits

![Logo](WTTJ_Logo_Black_RGB.png)

**Welcome dear \<reader>!**

**Every week, we, as the engineering team at Welcome to the Jungle, will share news about our tech products as well as details about the technical topics we've been working on. The newsletter, called Welcome Bits, will also include a curated list of the most interesting links we found out there in the wild wild web.**

<details>
<summary>What is Welcome to the Jungle</summary>
<p>

<a href="https://www.welcometothejungle.com/fr">Welcome to the Jungle</a> is a company creating the new experience at work. We use content and technology to transform every step of the employee experience to help companies offer a better, more human experience in the workplace.</p>
</details>

<details>
<summary>Why we decided to create Welcome Bits</summary>
<p>
  
Learning and sharing knowledge is part of the engineering team DNA. Since the beginning, Jungle Labs sessions are for instance organized each month so that developers in the team can spend a day away from their daily tasks to learn new stuff, grow technically, and share it with the rest of the team (which is not always an easy exercice for the shyest people among us).

So it seemed part of a continuing process to extend this learning and sharing experience to the outside world, meaning you, dear readers. And we hope you will enjoy reading it as much as we enjoyed writing it!</p>
</details>

<details>
<summary>The engineering team behind Welcome Bits</summary>
<p>
  
We are currently 14 developers in the engineering team itself, which is part of a bigger team called (what a surprise) "the tech team" where there are also product, data, design and QA people.

There are unfortunately only men right now in the engineering team, but as diversity is a value dear to our heart, our tech recruiter Xavier is working hard to hire women. If you are a woman who code, please check <a href="https://www.welcometothejungle.com/fr/companies/wttj/jobs">our current opened positions</a> and apply if you are interested!

The company is based in Paris, France, but 65% of us are working in full remote mode, which means that some of us can code while enjoying a beautiful view on the mountains or the ocean.

The team is composed of back-end, full-stack and front-end developers, as well as one devOps engineer and one head of engineering. We are working with Elixir, Ruby and React JS among others (you can check <a href="https://www.welcometothejungle.com/fr/companies/wttj/tech">our full stack</a> for more details).

If you want to know more about our team and the tech team in general, take a look at <a href="https://youtu.be/9QAV5r-sFhI">the filmed interview of Kevin</a>, our beloved CTO.</p>
</details>

*This newsletter is quite new, so your suggestions, questions and comments are more than welcome! Send us an issue or a pull request to do so.*

# Welcome Bits #1

## Bits of learning

"Optimizing your database the right way is never a waste of time"

> The last couple of weeks, we have been experiencing 40+ millions IOPS in some of our databases. Our first instinct was to check if any microservice was responsible for the high throughput, then we investigated AWS replicas and finally we went after all the releases that were made in the last 6 months to look for any breaking change. But the answer to our performance issues was not there... So we started to look closer at the databases. We identified a lack of optimisation and relevant indexes, and started to log slow queries and implement [pghero](https://github.com/ankane/pghero). After a few optimizations, we managed to divide by two our IOPS on our main database!

*By Thomas, head of engineering*

## Bits of content

[Pomerium](https://github.com/pomerium/pomerium) [![Generic badge](https://img.shields.io/badge/-OpenVPN%20alternative-brightgreen)]() [![Generic badge](https://img.shields.io/badge/-Kubernetes%20API%20Proxy-blue)]() [![Generic badge](https://img.shields.io/badge/-Identity%20and%20policy%20management-red)]()
<Details>
  <Summary>Details</Summary>
  <p>
    
*By Charles, devOps engineer*
    
> I was looking for a way to install a VPN to access our preproduction environment. We currently need multiple logins and passwords to access it, which is painful,    and some of my teammates have dynamic public IPs, so this kind of filter can't be used either. I already knew the solution OpenVPN but it required to install additional tools to be able to manage identity aspects and policies access. That's how I found out pomerium that seems promising, as it is more comprehensive and has a Kubernetes API proxy.
  </p>
</Details>

[The styled-components happy path](https://www.joshwcomeau.com/css/styled-components/) [![Generic badge](https://img.shields.io/badge/-Josh%20Comeau-yellow)]() [![Generic badge](https://img.shields.io/badge/-Lighter%20CSS%20files-red)]() [![Generic badge](https://img.shields.io/badge/-CSS%20variables-blue)]() [![Generic badge](https://img.shields.io/badge/-Single%20source%20of%20styles-brightgreen)]()
<Details>
  <Summary>Details</Summary>
  <p>
    
*By François, front-end developer*
    
> I really like Josh Comeau's blog posts about React and CSS because they are at a time qualitative, simple and interactive. His latest article about the best practices for styled-components was in particular very useful to me as it presents ways to lighten and simplify CSS files thanks to CSS variables and single source of styles.
  </p>
</Details>

[Jam](https://jam.dev) [![Generic badge](https://img.shields.io/badge/-Building%20websites-brightgreen)]() [![Generic badge](https://img.shields.io/badge/-Collaborative-yellow)]() [![Generic badge](https://img.shields.io/badge/-Beta-lightgrey)]()

[Improving how we deploy GitHub](https://github.blog/2021-01-25-improving-how-we-deploy-github/) [![Generic badge](https://img.shields.io/badge/-Slack-blue)]() [![Generic badge](https://img.shields.io/badge/-Overview%20of%20deploys-red)]() [![Generic badge](https://img.shields.io/badge/-Automation-brightgreen)]()

[How (some) good corporate engneering blogs are written](https://danluu.com/corp-eng-blogs/) [![Generic badge](https://img.shields.io/badge/-Engineering%20blogs-brightgreen)]() [![Generic badge](https://img.shields.io/badge/-Best%20practices-yellow)]() [![Generic badge](https://img.shields.io/badge/-Cloudflare-blue)]() [![Generic badge](https://img.shields.io/badge/-Segment-lightgrey)]() [![Generic badge](https://img.shields.io/badge/-Heap-red)]()

## Bits of good vibes

Our open-source customizable design system with react styled-components, styled-system and reakit, named [Welcome UI](https://github.com/WTTJ/welcome-ui), just reached 248 stars on GitHub! Don't hesitate to use it and/or contribute.

## Bits of jobs

There are currently 5 positions opened in the engineering team:

[Engineering manager](https://www.welcometothejungle.com/en/companies/wttj/jobs/engineering-manager_paris)

[DevOps engineer](https://www.welcometothejungle.com/en/companies/wttj/jobs/devops-engineer_paris)

[Full Stack developer (Elixir, Ruby, React JS)](https://www.welcometothejungle.com/en/companies/wttj/jobs/full-stack-developer-ruby-elixir-react-js_paris)

[Back-end developer (Elixir, Ruby)](https://www.welcometothejungle.com/en/companies/wttj/jobs/backend-developer-ruby-elixir_paris_WTTJ_9MP4PxM)

[Front-end developer (React JS, CSS-in-JS)](https://www.welcometothejungle.com/en/companies/wttj/jobs/frontend-developer-react-js-css-in-js_paris)

If you have any question about the positions, send us an issue or a pull request!


Thanks for reading us. Don't hesitate to open an issue or a pull request for any question or comment you may have about the newsletter or one of the opened position. We will answer you as soon as we can. See you next week!
