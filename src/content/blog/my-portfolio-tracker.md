---
title: My personal portfolio tracker
description: 
pubDate: 2026-05-06
tags: ["web app"]
---

My wife and I have multiple investment accounts. Over the years, I’ve tried several applications to track our portfolio and performance, but I’ve always wanted a lightweight tool that can consolidate everything in one place.

Here are a few solutions I explored.

## Morningstar Portfolio Manager

Morningstar Portfolio Manager is an investment analysis and portfolio tracking tool offered by Morningstar.

### Pros:
- Free to use  
- Supports stocks, ETFs, mutual funds, bonds, and more, with strong analytics and reporting  
- Automatically tracks events like stock splits and dividends  

### Cons:
- When combining multiple accounts into one portfolio, it cannot track cash balances per account  
- Does not support options  
- Not mobile-friendly  

## Empower Web

Empower allows you to link multiple financial accounts and view everything in a single dashboard.

### Pros:
- Supports stocks, ETFs, mutual funds, bonds, options, and more  
- Provides strong BI-style reports for portfolio analysis  

### Cons:
- Not truly free, you need an Empower account  
- The mobile app does not show linked accounts  
- Feels heavy and slow  

## Ghostfolio

Ghostfolio is an open-source portfolio tracking web application.

### Pros:
- Open source and self-hostable  
- Fast and responsive  
- Provides essential portfolio analysis features  

### Cons:
- Does not support options out of the box  
- Overkill for a simple, single-user use case like mine  

---

## Building My Own

After trying these tools, I decided to build my own portfolio tracker. My goals were simple: **lightweight, fast, cheap, and easy to use**.

Here’s the tech stack I chose:

- **Database**: AWS DynamoDB  
- **Backend**: AWS Lambda  
- **API**: AWS API Gateway  
- **Authentication**: AWS Cognito  
- **Frontend**: React.js + Tailwind CSS  
- **Hosting**: AWS S3 (static site)  
- **Deployment**: AWS CDK  

With the help of GitHub Copilot (free tier), development moved faster than expected. After about two weeks of casual work, I had a working prototype live.

![screen](/blog_assets/pt-screen.png)  
*(Note: the numbers shown are not real.)*

There’s still a lot to improve, but it’s been fun building something useful, especially with AI accelerating the process.

You can find the repository here:  
👉 [portfolio tracker](https://github.com/chongtian/portfolio-tracker)
