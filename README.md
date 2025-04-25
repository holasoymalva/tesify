# ThesisBuilder

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-1.0.0-green.svg)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)

> A research assistant for PhD students that helps develop robust thesis statements by analyzing existing literature and identifying research gaps.

## 🚀 Overview

ThesisBuilder is an AI-powered research assistant designed specifically for PhD students and academic researchers. By leveraging the Perplexity API and advanced NLP techniques, ThesisBuilder streamlines the literature review process, identifies research gaps, and helps formulate compelling thesis statements with strong academic foundations.

**Key Features:**
- Literature analysis across multiple academic databases
- Research gap identification using semantic analysis
- Thesis statement generation and refinement
- Citation management and recommendation
- Methodology suggestion based on research questions

## 📊 Demo

![ThesisBuilder Demo](./assets/thesisbuilder-demo.gif)

Try the live demo: [ThesisBuilder Demo](https://tesify-demo.vercel.app)

## 🛠️ Tech Stack

- **Frontend:**
  - React.js with TypeScript
  - Next.js for server-side rendering
  - Tailwind CSS for styling
  - React Query for data fetching

- **Backend:**
  - Node.js with Express
  - MongoDB for database
  - Redis for caching

- **AI/ML:**
  - Perplexity API for knowledge retrieval and synthesis
  - NLP processing pipeline for academic text analysis
  - Vector embeddings for semantic similarity analysis

- **DevOps:**
  - Docker for containerization
  - GitHub Actions for CI/CD
  - AWS for hosting
  - Vercel for frontend deployment

## 📋 Prerequisites

- Node.js (v16+)
- MongoDB (v5+)
- Redis (v6+)
- Perplexity API key
- Docker (optional, for containerized deployment)

## ⚙️ Installation

1. Clone the repository:
```bash
git clone https://github.com/holasoymalva/tesify.git
cd tesify
```

2. Install dependencies:
```bash
# Install backend dependencies
cd server
npm install

# Install frontend dependencies
cd ../client
npm install
```

3. Set up environment variables:
```bash
# In the server directory
cp .env.example .env
```

4. Update the `.env` file with your credentials:
```
PORT=8000
MONGODB_URI=mongodb://localhost:27017/thesisbuilder
REDIS_URL=redis://localhost:6379
PERPLEXITY_API_KEY=your_perplexity_api_key
JWT_SECRET=your_jwt_secret
```

5. Start the development servers:
```bash
# Start backend server
cd server
npm run dev

# Start frontend development server
cd ../client
npm run dev
```

6. Open your browser and navigate to `http://localhost:3000`

## 🐳 Docker Setup

```bash
# Build and run with Docker Compose
docker-compose up -d
```

## 📚 API Documentation

The API documentation is available at `/api-docs` when running the server locally, or at [https://tesify-api.vercel.app/api-docs](https://tesify-api.vercel.app/api-docs) for the production environment.

### Key Endpoints

- `POST /api/analyze` - Analyze research papers
- `POST /api/gaps` - Identify research gaps
- `POST /api/thesis/generate` - Generate thesis statement
- `GET /api/citations` - Get citation recommendations

## 🔎 How It Works

ThesisBuilder follows a multi-step process to help researchers develop robust thesis statements:

1. **Literature Collection:** Aggregates relevant papers from academic databases based on your research interests.
2. **Content Analysis:** Uses the Perplexity API to deeply analyze the content, methodology, and findings of each paper.
3. **Gap Identification:** Employs semantic analysis to identify unexplored areas and contradictions in existing literature.
4. **Thesis Generation:** Creates potential thesis statements that address identified gaps.
5. **Refinement:** Collaboratively refines thesis statements through iterative feedback.

## 🧪 Testing

```bash
# Run backend tests
cd server
npm test

# Run frontend tests
cd client
npm test

# Run end-to-end tests
npm run test:e2e
```

## 🛣️ Roadmap

- [ ] Integration with additional academic databases
- [ ] Advanced visualization of research landscape
- [ ] Collaborative thesis workspaces for research teams
- [ ] Methodology recommendation engine
- [ ] Automated literature review drafting
- [ ] Integration with reference managers (Zotero, Mendeley)

## 👥 Contributing

We welcome contributions to ThesisBuilder! Please read our [contributing guidelines](CONTRIBUTING.md) before submitting a pull request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgements

- [Perplexity AI](https://www.perplexity.ai) for their powerful API
- The open-source NLP community
- All academic researchers who provided feedback during the development process

## 📞 Contact

For questions or feedback, please reach out:

- GitHub: [@holasoymalva](https://github.com/holasoymalva)
- Email: team@tesify.dev
- Twitter: [@ThesisBuilderAI](https://twitter.com/ThesisBuilderAI)

---

Made with ❤️ for researchers by researchers
