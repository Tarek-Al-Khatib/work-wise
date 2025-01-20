<img src="./readme/title1.svg"/>

<br><br>

<!-- project philosophy -->
<img src="./readme/title2.svg"/>

> Workwise is an AI-driven platform designed to empower users in their career growth and development, providing personalized learning paths, mock interview simulations, and community collaboration to help them achieve their professional goals.
>
> The project aims to streamline career advancement by offering tailored learning plans, realistic interview experiences, and fostering a supportive community for networking, mentorship, and skill development. We believe in enhancing career journeys by making learning and professional growth more accessible, engaging, and effective.

## User Stories

### User

- As a user, I want to create a personalized learning plan and track the progress, so I can work towards my career goals step by step.
- As a user, I want to participate in mock interviews with AI or Moderator, so I can practice and improve my interview skills.
- As a user, I want to join a community, so I can collaborate with like-minded individuals and gain mentorship.

### Moderator

- As a moderator, I want to check the pending invitations that are sent to me for mock interviews
- As a moderator, I want to give a detailed feedback after each interview is completed, and I want to accept or reject interviews invitations.
- As a moderator, I am designated as the person users conduct interviews with in the community, ensuring that I can actively support their preparation and provide valuable feedback.

### Admin

- As an admin, I want to assign moderator roles to community members, so I can ensure the community is actively managed and moderated.
- As an admin, I want to create new channels within the community, so users can engage in focused discussions based on specific topics or interests.
- As an admin, I want to edit community details, such as the name, description, or rules, so I can keep the community's information accurate and up-to-date.

<br><br>

<!-- Tech stack -->
<img src="./readme/title3.svg"/>

### WorkWise is built using the following technologies:

- The project uses [ReactJS](https://react.dev/) for the frontend, enabling an interactive and dynamic user interface.
- For the backend server, it utilizes [Node.js](https://nodejs.org/en) with [Express.js](https://expressjs.com/), providing a robust and scalable API.
- The platform relies on [MySQL](https://www.mysql.com/) for relational database management, ensuring efficient data storage and retrieval.
- For real-time features, the project integrates [Socket.io](https://socket.io/), enabling live notifications and updates across the platform.
- Advanced 3D visualizations are powered by [Three.js](https://threejs.org/), offering immersive and interactive experiences.
- Seamless video conferencing capabilities are achieved using [Daily.js](https://www.daily.co/).

  <br><br>

<!-- UI UX -->
<img src="./readme/title4.svg"/>

> WorkWise started as simple wireframes and mockups. We kept refining the design, taking feedback at every step, until it felt just right to use, fun to navigate, and perfectly suited to help users grow their careers.

- Project Figma design [figma](https://www.figma.com/design/zplq3EtGiAvkY5so23DcGL/WorkWise-Wireframes?node-id=0-1&t=DDK6dIZuo9VDnyA6-1)

### Mockups

| My Interviews screen                               | Profile Screen                           |
| -------------------------------------------------- | ---------------------------------------- |
| ![InterviewScreen](./readme/mockups/interview.png) | ![Profile](./readme/mockups/profile.png) |

<br><br>

<!-- Database Design -->
<img src="./readme/title5.svg"/>

### Architecting Data Excellence: Innovative Database Design Strategies:

<img src="./readme/DBDiagram/WorkWise_DBDiagram.png"/>

<br><br>

<!-- Implementation -->
<img src="./readme/title6.svg"/>

### User Screens

| AI Interview screen                                | Communities screen                                   |
| -------------------------------------------------- | ---------------------------------------------------- |
| ![AIInterview](./readme/screens/ai_interview.gif)  | ![Communities](./readme/screens/community_page.gif)  |
| Dashboard screen                                   | My Interviews Screen                                 |
| ![Dashboard](./readme/screens/dashboard_video.gif) | ![MyInterviews](./readme/screens/interview_page.gif) |
| My Learning screen                                 | Video Call Screen                                    |
| ![MyLearning](./readme/screens/learning_page.gif)  | ![VideoCall](./readme/screens/video_call_page.gif)   |
| Add New Plan screen                                | Profile screen                                       |
| ![NewPlan](./readme/mockups/add_learning.png)      | ![Profile](./readme/mockups/profile.png)             |

### Admin Screens

| Create Community                                  | Create Channel                                 |
| ------------------------------------------------- | ---------------------------------------------- |
| ![MyLearning](./readme/mockups/add_community.png) | ![VideoCall](./readme/mockups/add_channel.png) |

<br><br>

<!-- Prompt Engineering -->
<img src="./readme/title7.svg"/>

### Mastering AI Interaction: Unveiling the Power of Prompt Engineering:

- This project uses advanced techniques to improve how we interact with OpenAI models. By carefully creating input instructions, we can guide the models to understand and generate language more accurately and efficiently for different tasks and needs.

  | Start interviewing                              | Complete Interview                                 |
  | ----------------------------------------------- | -------------------------------------------------- |
  | ![StartInterview](./readme/prompts/prompt1.png) | ![CompleteInterview](./readme/prompts/prompt4.png) |
  | Enhance Plan                                    | Create Top Picks                                   |
  | ![NewPlan](./readme/prompts/prompt2.png)        | ![Profile](./readme/prompts/prompt3.png)           |

<br><br>

<!-- AWS Deployment
<img src="./readme/title8.svg"/>

### Efficient AI Deployment: Unleashing the Potential with AWS Integration:

- This project leverages AWS deployment strategies to seamlessly integrate and deploy natural language processing models. With a focus on scalability, reliability, and performance, we ensure that AI applications powered by these models deliver robust and responsive solutions for diverse use cases.

<br><br> -->

<!-- Unit Testing -->
<!-- <img src="./readme/title9.svg"/>

### Precision in Development: Harnessing the Power of Unit Testing:

- This project employs rigorous unit testing methodologies to ensure the reliability and accuracy of code components. By systematically evaluating individual units of the software, we guarantee a robust foundation, identifying and addressing potential issues early in the development process.

<br><br> -->

<!-- How to run -->
<img src="./readme/title10.svg"/>

> To set up WorkWise locally, follow these steps:

## Installation

1. Get a free API Key at [ElevenLabs](https://elevenlabs.io/), [DailyJS](https://www.daily.co/), and [NINJASAPI](https://www.api-ninjas.com/)
2. Get an API key at [OPENAI](https://openai.com/index/openai-api/)
3. Clone the repo
   git clone [github](https://github.com/Tarek-Al-Khatib/work-wise)

### Backend Side

1. Install NPM packages
   ```sh
   npm install
   ```
2. Run the following commands
   ```sh
   npx prisma migrate dev
   npm run prisma:seed
   ```
3. Enter your API keys, secrets, and configurations in `.env`
   ```env
   DATABASE_URL="Your MySQL server connection"
   PORT=Enter your Preffered port
   JWT_SECRET="Enter your JWT Secret key"
   DAILY_API_KEY="Enter your Daily JS free API key"
   OPENAI_API_KEY="Enter your Open AI API key"
   ELEVEN_LABS_API_KEY="Enter your ElevenLabs free API key"
   ```

### Frontend Side

1. Install NPM Packages

   ```sh
   npm install --legacy-peer-deps
   ```

2. Enter your API key for NINJA'S API

   ```env
   REACT_APP_NINJAS_API="Enter your NINJAS API free API key"
   ```

3. Put your server URL inside of src -> config -> url.js

   ```js
   export const serverUrl = "Your Server URL";
   ```

Now, you should be able to run WorkWise locally and explore its features.
