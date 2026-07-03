<div align="center">
  <img src="public/favicon.ico" alt="PokeSearch Logo" width="50"/>
  
  # Resume.GPT

  **A web application that functions as an AI-powered resume reviewer. It allows users to upload their resumes, such as PDFs, to receive an Applicant Tracking System (ATS) compatibility score, feedback badges, and a detailed summary of their document's effectiveness.**
  
  [![React](https://img.shields.io/badge/React-ffffff.svg?style=flat&logo=react)](https://reactjs.org/)
  [![React](https://img.shields.io/badge/React_Router_v7-ffffff.svg?style=flat&logo=react)](https://reactjs.org/)
  [![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-ffffff.svg?style=flat&logo=tailwind-css)](https://tailwindcss.com/)
  [![Typescript](https://img.shields.io/badge/TypeScript-ffffff.svg?style=flat&logo=typescript)](https://tailwindcss.com/)
  [![Puter.js](https://img.shields.io/badge/Puter.js-ffffff.svg?style=flat&logo=javascript)](https://tailwindcss.com/)
</div>

## 📖 About this Project
Many people never consider how their resume looks like to hiring managers and often would mass-apply to jobs in which they truly don't know what the requirements are, and in other cases, it specifically because the resumes dont outshine others when scanned through the ATS (applicant tracking system). This is where Resume.GPT

## 🌐 Try it Out!
https://ai-resume-reviewer-beta.vercel.app/

## 🛠️ Technologies Used
- **Frontend Framework:** React (v19), Vite, React Router v7, Tailwind CSS v4, Tailwind Animate Node.js
- **State Management:** Zustand
- **Backend:** Puter.js (providing serverless authentication, cloud file storage, key-value storage, and AI integrations), PDF.js
- **AI Model:** Claude Sonnet 4.6
- **Utilities:** CLSX, Tailwind Merge

## ⭐ Key Features
- Secure user authentication with Puter.js
- Responsive Design: Fully optimized for mobile, tablet, and desktop views.
- Uses Claude models to scan and analyze resume documents to display helpful and detailed feedback based on the user's job application
- Secure cloud storage management via Puter to store scanned resumes under the user's account

## 🗯️ Lessons Learned
- Challenge: I struggled with trying to have the AI model output to areas needed, which also caused me to reach AI token limits
- Solution: Using prompt engineering, I have made a detailed test prompt to guide the AI model to bring valid JSON data, making the app 50% more efficient than before
- Future Improvements: I plan to add Dark Mode Toggle to this app and build a page to clear out user's data to increase the functionality of this app.

## 📝 Prerequisites

- [Node.js](https://nodejs.org/en/) (v20.19.0 or higher recommended)
- `npm` or `yarn`
- Docker (optional, for containerized deployment)

## 🚀 Getting Started

### Installation

Install the dependencies:

```bash
npm install
```

### Development

Start the development server with HMR:

```bash
npm run dev
```

Your application will be available at `http://localhost:5173`.

## Building for Production

Create a production build:

```bash
npm run build
```

## Deployment

### Docker Deployment

To build and run using Docker:

```bash
docker build -t my-app .

# Run the container
docker run -p 3000:3000 my-app
```

The containerized application can be deployed to any platform that supports Docker, including:

- AWS ECS
- Google Cloud Run
- Azure Container Apps
- Digital Ocean App Platform
- Fly.io
- Railway

### DIY Deployment

If you're familiar with deploying Node applications, the built-in app server is production-ready.

Make sure to deploy the output of `npm run build`

```
├── package.json
├── package-lock.json (or pnpm-lock.yaml, or bun.lockb)
├── build/
│   ├── client/    # Static assets
│   └── server/    # Server-side code
```

## 📁 Project Structure
```
ai_resume_reviewer/
├── .dockerignore
├── .gitignore
├── Dockerfile
├── README.md
├── package-lock.json
├── package.json
├── react-router.config.ts
├── tsconfig.json
├── vite.config.ts
├── app/
│   ├── app.css
│   ├── root.tsx
│   ├── routes.ts
│   ├── components/
│   │   ├── ATS.tsx
│   │   ├── Accordion.tsx
│   │   ├── Details.tsx
│   │   ├── FileUploader.tsx
│   │   ├── Navbar.tsx
│   │   ├── ResumeCard.tsx
│   │   ├── ScoreBadge.tsx
│   │   ├── ScoreCircle.tsx
│   │   ├── ScoreGauge.tsx
│   │   └── Summary.tsx
│   ├── lib/
│   │   ├── pdf2img.ts
│   │   ├── puter.ts
│   │   └── utils.ts
│   └── routes/
│       ├── auth.tsx
│       ├── home.tsx
│       ├── resume.tsx
│       ├── upload.tsx
│       └── wipe.tsx
├── constants/
│   └── index.ts
├── public/
│   ├── favicon.ico
│   ├── pdf.worker.min.mjs
│   ├── icons/
│   │   ├── ats-bad.svg
│   │   ├── ats-good.svg
│   │   ├── ats-warning.svg
│   │   ├── back.svg
│   │   ├── check.svg
│   │   ├── cross.svg
│   │   ├── info.svg
│   │   ├── pin.svg
│   │   └── warning.svg
│   └── images/
│       ├── bg-auth.svg
│       ├── bg-main.svg
│       ├── bg-small.svg
│       ├── pdf.png
│       ├── resume-scan-2.gif
│       ├── resume-scan.gif
│       ├── resume_01.png
│       ├── resume_02.png
│       ├── resume_03.png
│       ├── resume_04.png
│       ├── resume_05.png
│       └── resume_06.png
└── types/
    ├── index.d.ts
    └── puter.d.ts
```

## 👥 Contributing
1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test throughly
5. Submit a pull request

## 📄 License
This project is open-source and available under the MIT License.

<div align="center">

## Contact
Have a project in mind? I'd love to hear about it! Check out my other work here!

[![Portfolio](https://img.shields.io/badge/My%20Portfolio-002500.svg?style=for-the-badge&logo=instatus&logoColor=white)](https://yyportfolio-xi.vercel.app/) [![LinkedIn](https://img.shields.io/badge/LinkedIn-002500.svg?style=for-the-badge&logo=instatus&logoColor=white)](https://www.linkedin.com/in/yasir-younus-91551a281) [![Gmail](https://img.shields.io/badge/Email-002500?style=for-the-badge&logo=gmail&logoColor=white)](mailto:yyproton168@gmail.com)
</div>