# Take Home Exercise: Slack Bot 🤖

## Objective:

Develop an interactive dashboard and Slack bot that integrates with OpenAI’s GPT API to provide intelligent, context-aware responses to user queries. The dashboard should offer insights into query trends, user engagement, and common topics, serving as a monitoring and analytics tool for interactions with the bot.

You are expected to spend up to 48 hours on the exercise, and you are *not* expected to complete all of the requirements below. Given the scope of features, you will need to prioritize, design, and develop key functionalities, making thoughtful trade-offs to deliver a well-structured, high-impact solution.

As an AI-first company, we encourage the use of tools like Cursor, ChatGPT, and other AI-assisted development resources to enhance efficiency and productivity.

## Requirements:

### **Backend:**

- **Slack Integration:**
    - Set up a bot that listens to messages in a Slack channel.
    - The bot should first attempt to answer questions based on past Slack threads before falling back to general knowledge from OpenAI’s GPT model.
- **OpenAI API Integration:**
    - Process user queries and generate appropriate responses.
    - Support retrieval-augmented generation (RAG) by leveraging relevant past conversations and tools like [pinecone.io](http://pinecone.io).
- **Uploaded Files as Context:**
    - Allow users to upload files that the model can reference when answering questions.
    - Extract text from uploaded documents (e.g., PDFs, CSVs, or text files) and include this information in query responses.
- **Data Logging & Storage:**
    - Store query data, responses, timestamps, and metadata to generate insights.
    - Store Slack messages for historical context and better query responses.

### **Frontend (Dashboard UI):**

- **React-Based Interface:**
    - Use React (TypeScript preferred) with Next.js, Vite, etc. for frontend development.
    - Build a responsive and interactive UI for monitoring query insights.
- **Metrics Dashboard:**
    
    Display key statistics on the queries made via the Slack bot, including:
    
    - **Hot Keywords:** Show the most frequently used keywords across all queries.
    - **Trend Over Time:** Chart how query volume and keyword popularity change over time.
    - **Top Users:** Rank users by the number of queries made.
    - **User Query Trends:** Show individual user engagement trends over time.
    - **Response Effectiveness:** Track how often the bot resolves queries without requiring human intervention.
- **Chat Interface:**
    - Enable users to interact with the bot directly via the dashboard.
    - Provide a chat history with timestamps, showing past queries and responses.
    - Allow users to input queries and get responses without using Slack.
- **File Upload & Context Usage:**
    - Implement a file upload feature to let users provide additional context for queries.
    - Display uploaded files and allow users to see how they influence responses.
- **Slack Message Summarization:**
    - Display summarized Slack conversations and extracted insights.
    - Provide a searchable history of Slack conversations relevant to specific keywords.

### **Nice-to-Have’s:**

- **Testing:**
    - Write unit and/or integration tests for both frontend and backend.
- **Deployment:**
    - Deploy frontend using Vercel and backend using Heroku/AWS/GCP.
- **Authentication:**
    - Implement basic authentication via Slack OAuth or simple login.
- **Additional Features:**
    - It’s really up to your imagination. Sky is the limit!

We are very excited to see what you can accomplish with this exercise. Most importantly, have fun with it!

👉 When completed, please reach out to Charles ([charles@vibraniumlabs.ai](mailto:charles@vibraniumlabs.ai)), cc Jay ([jay@vibraniumlabs.ai](mailto:jay@vibraniumlabs.ai)) and Reese ([reese@t1.co](mailto:reese@t1.co)) and share the link to your repository for the exercise. Charles will then set up a 30 minute debrief/demo. Good luck!

---

<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="120" alt="Nest Logo" /></a>
</p>

[circleci-image]: https://img.shields.io/circleci/build/github/nestjs/nest/master?token=abc123def456
[circleci-url]: https://circleci.com/gh/nestjs/nest

  <p align="center">A progressive <a href="http://nodejs.org" target="_blank">Node.js</a> framework for building efficient and scalable server-side applications.</p>
    <p align="center">
<a href="https://www.npmjs.com/~nestjscore" target="_blank"><img src="https://img.shields.io/npm/v/@nestjs/core.svg" alt="NPM Version" /></a>
<a href="https://www.npmjs.com/~nestjscore" target="_blank"><img src="https://img.shields.io/npm/l/@nestjs/core.svg" alt="Package License" /></a>
<a href="https://www.npmjs.com/~nestjscore" target="_blank"><img src="https://img.shields.io/npm/dm/@nestjs/common.svg" alt="NPM Downloads" /></a>
<a href="https://circleci.com/gh/nestjs/nest" target="_blank"><img src="https://img.shields.io/circleci/build/github/nestjs/nest/master" alt="CircleCI" /></a>
<a href="https://discord.gg/G7Qnnhy" target="_blank"><img src="https://img.shields.io/badge/discord-online-brightgreen.svg" alt="Discord"/></a>
<a href="https://opencollective.com/nest#backer" target="_blank"><img src="https://opencollective.com/nest/backers/badge.svg" alt="Backers on Open Collective" /></a>
<a href="https://opencollective.com/nest#sponsor" target="_blank"><img src="https://opencollective.com/nest/sponsors/badge.svg" alt="Sponsors on Open Collective" /></a>
  <a href="https://paypal.me/kamilmysliwiec" target="_blank"><img src="https://img.shields.io/badge/Donate-PayPal-ff3f59.svg" alt="Donate us"/></a>
    <a href="https://opencollective.com/nest#sponsor"  target="_blank"><img src="https://img.shields.io/badge/Support%20us-Open%20Collective-41B883.svg" alt="Support us"></a>
  <a href="https://twitter.com/nestframework" target="_blank"><img src="https://img.shields.io/twitter/follow/nestframework.svg?style=social&label=Follow" alt="Follow us on Twitter"></a>
</p>
  <!--[![Backers on Open Collective](https://opencollective.com/nest/backers/badge.svg)](https://opencollective.com/nest#backer)
  [![Sponsors on Open Collective](https://opencollective.com/nest/sponsors/badge.svg)](https://opencollective.com/nest#sponsor)-->

## Description

[Nest](https://github.com/nestjs/nest) framework TypeScript starter repository.

## Project setup

```bash
$ npm install
```

## Compile and run the project

```bash
# development
$ npm run start

# watch mode
$ npm run start:dev

# production mode
$ npm run start:prod
```

## Run tests

```bash
# unit tests
$ npm run test

# e2e tests
$ npm run test:e2e

# test coverage
$ npm run test:cov
```

## Deployment

When you're ready to deploy your NestJS application to production, there are some key steps you can take to ensure it runs as efficiently as possible. Check out the [deployment documentation](https://docs.nestjs.com/deployment) for more information.

If you are looking for a cloud-based platform to deploy your NestJS application, check out [Mau](https://mau.nestjs.com), our official platform for deploying NestJS applications on AWS. Mau makes deployment straightforward and fast, requiring just a few simple steps:

```bash
$ npm install -g mau
$ mau deploy
```

With Mau, you can deploy your application in just a few clicks, allowing you to focus on building features rather than managing infrastructure.

## Resources

Check out a few resources that may come in handy when working with NestJS:

- Visit the [NestJS Documentation](https://docs.nestjs.com) to learn more about the framework.
- For questions and support, please visit our [Discord channel](https://discord.gg/G7Qnnhy).
- To dive deeper and get more hands-on experience, check out our official video [courses](https://courses.nestjs.com/).
- Deploy your application to AWS with the help of [NestJS Mau](https://mau.nestjs.com) in just a few clicks.
- Visualize your application graph and interact with the NestJS application in real-time using [NestJS Devtools](https://devtools.nestjs.com).
- Need help with your project (part-time to full-time)? Check out our official [enterprise support](https://enterprise.nestjs.com).
- To stay in the loop and get updates, follow us on [X](https://x.com/nestframework) and [LinkedIn](https://linkedin.com/company/nestjs).
- Looking for a job, or have a job to offer? Check out our official [Jobs board](https://jobs.nestjs.com).

## Support

Nest is an MIT-licensed open source project. It can grow thanks to the sponsors and support by the amazing backers. If you'd like to join them, please [read more here](https://docs.nestjs.com/support).

## Stay in touch

- Author - [Kamil Myśliwiec](https://twitter.com/kammysliwiec)
- Website - [https://nestjs.com](https://nestjs.com/)
- Twitter - [@nestframework](https://twitter.com/nestframework)

## License

Nest is [MIT licensed](https://github.com/nestjs/nest/blob/master/LICENSE).
