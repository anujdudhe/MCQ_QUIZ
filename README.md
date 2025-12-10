# GE Civil MCQ Exam App

[![Netlify Status](https://api.netlify.com/api/v1/badges/your-site-id/deploy-status)](https://app.netlify.com/sites/ge-mcq/overview)

A modern, responsive Multiple Choice Question (MCQ) exam application for GE Civil Engineering students. Built with React, TypeScript, and Tailwind CSS, this application allows users to take timed exams, review their answers, and see detailed results.

🌐 **Live Demo**: [https://ge-mcq.netlify.app](https://ge-mcq.netlify.app)

## Features

- 📝 Interactive exam interface with multiple-choice questions
- ⏱️ Timer to track exam duration
- 📊 Real-time progress tracking
- 🔍 Question navigation and review
- 📱 Responsive design for all screen sizes
- 📝 Support for various question formats
- 📊 Detailed exam results and performance analysis

## Prerequisites

- Node.js (v16 or higher)
- npm (v7 or higher) or yarn

## Getting Started

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/mcq-exam-app.git
   cd mcq-exam-app
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
   ```

3. **Start the development server**
   ```bash
   npm run dev
   # or
   yarn dev
   ```

4. **Open in your browser**
   The application will be available at `http://localhost:5173`

## Project Structure

```
GE-Civil-MCQ/
├── src/
│   ├── components/     # Reusable UI components
│   │   ├── ModalIntro.tsx  # Introduction modal component
│   │   ├── QuestionCard.tsx  # Question display component
│   │   ├── ProgressBar.tsx  # Progress indicator
│   │   ├── Result.tsx      # Results display
│   │   └── ...
│   ├── data/          # Question data and utilities
│   ├── types/         # TypeScript type definitions
│   ├── App.tsx        # Main application component
│   └── main.tsx       # Application entry point
├── public/            # Static assets
├── scripts/           # Utility scripts for question processing
│   ├── pdf-to-json.js # Convert PDF question bank to JSON
│   └── verify-questions.js # Verify question data integrity
├── package.json       # Project dependencies and scripts
├── netlify.toml       # Netlify deployment configuration
└── vite.config.ts     # Vite configuration
```

## 🛠 Available Scripts

### Development
- `npm run dev` - Start the development server
- `npm run preview` - Preview the production build locally

### Build
- `npm run build` - Build the application for production

### Question Bank Management
- `npm run convert-pdf` - Convert PDF question bank to JSON format
- `npm run verify-questions` - Verify the integrity of question data

### Deployment
- `netlify deploy` - Deploy to Netlify (staging)
- `netlify deploy --prod` - Deploy to production

## Adding Questions

1. Place your PDF question bank in the root directory
2. Run the conversion script:
   ```bash
   npm run convert-pdf
   ```
3. The converted questions will be available in the `src/data` directory

## Customization

### Styling
This project uses Tailwind CSS for styling. You can customize the design by modifying the `tailwind.config.js` file.

### Configuration
- Update `vite.config.ts` for build configurations
- Modify `tsconfig.json` for TypeScript settings

## 🚀 Deployment

This project is automatically deployed to Netlify on every push to the `main` branch.

### Manual Deployment

1. **Build the application**
   ```bash
   npm run build
   ```

2. **Deploy to Netlify**
   ```bash
   netlify deploy --prod
   ```

### Continuous Deployment
- The app is configured for automatic deployment via GitHub
- Pushing to the `main` branch triggers a new deployment
- Build settings are configured in `netlify.toml`

### Deployment Status
- **Production URL**: [https://ge-mcq.netlify.app](https://ge-mcq.netlify.app)
- **Admin Dashboard**: [Netlify Admin](https://app.netlify.com/sites/ge-mcq/overview)

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Built with [Vite](https://vitejs.dev/)
- Styled with [Tailwind CSS](https://tailwindcss.com/)
- Icons from [React Icons](https://react-icons.github.io/react-icons/)
