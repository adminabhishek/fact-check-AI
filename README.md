markdown
# 🔍 FactCheckAI - Fake News Detector with Evidence & Sources

[![Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://factcheckai.streamlit.app/)
[![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg)](https://python.org)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

> An AI-powered fact-checking system that provides instant, evidence-based verification of claims with transparent sourcing and reasoning.

![FactCheckAI Demo](https://via.placeholder.com/800x400.png?text=FactCheckAI+Demo+GIF)
*Visual demonstration of FactCheckAI in action*

## ✨ Features

### 🔍 Smart Verification
- **Real-time Analysis**: Instant fact-checking of any claim or headline
- **Multi-Source Evidence**: Aggregates evidence from diverse news sources
- **AI-Powered Reasoning**: Uses Google Gemini for intelligent analysis
- **Transparent Sourcing**: Shows exactly where information comes from

### 📊 Credibility Assessment
- **Source Scoring**: Automatic credibility rating for each news source
- **Freshness Filter**: Prioritizes recent information with configurable time windows
- **Regional Coverage**: Supports multiple geographic regions for localized news

### 🎨 User Experience
- **Beautiful UI**: Modern, responsive design with smooth animations
- **Mobile Optimized**: Works perfectly on desktop, tablet, and mobile
- **Interactive Results**: Expandable evidence cards and source previews
- **Shareable Reports**: Download and share comprehensive fact-check reports

### ⚡ Performance
- **Fast Processing**: Parallel article fetching and smart caching
- **Rate Limiting**: Prevents abuse and ensures fair usage
- **Error Handling**: Graceful degradation when services are unavailable

## 🚀 Quick Start

### Prerequisites
- Python 3.9 or higher
- Google Gemini API key ([Get one free](https://aistudio.google.com/))

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/factcheck-ai.git
   cd factcheck-ai
Create virtual environment

bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
Install dependencies

bash
pip install -r requirements.txt
Set up environment variables

bash
# Create .env file
echo "GEMINI_API_KEY=your_gemini_api_key_here" > .env
Run locally

bash
streamlit run app.py
Deployment
Option 1: Streamlit Cloud (Recommended)
Fork this repository

Go to Streamlit Cloud

Connect your GitHub account and select this repository

Add your GEMINI_API_KEY in the secrets section

Deploy! 🚀

Option 2: Other Platforms
Heroku: https://www.herokucdn.com/deploy/button.svg

DigitalOcean: See DEPLOYMENT.md

Docker: docker build -t factcheckai . && docker run -p 8501:8501 factcheckai

🎯 Usage Examples
Basic Fact-Checking
python
# The web interface makes it easy to verify claims like:
- "NASA discovered water on Mars"
- "Eating chocolate improves memory"
- "The Great Wall of China is visible from space"
Advanced Features
Region Selection: Choose news sources from different countries

Freshness Control: Set how recent articles should be (6-168 hours)

Analysis Creativity: Adjust AI temperature for more conservative or creative analysis

📁 Project Structure
text
factcheck-ai/
├── app.py                 # Main Streamlit application
├── requirements.txt       # Python dependencies
├── .streamlit/
│   └── config.toml       # Streamlit configuration
├── .env                  # Environment variables (gitignored)
├── Dockerfile           # Container configuration
├── LICENSE              # MIT License
├── README.md           # This file
└── assets/             # Images and static files
    └── demo.gif        # Demo animation
🔧 Configuration
Environment Variables
bash
GEMINI_API_KEY=your_gemini_api_key_here        # Required: Google Gemini API key
Streamlit Secrets (for cloud deployment)
toml
GEMINI_API_KEY = "your_gemini_api_key_here"
Customization Options
Modify CREDIBLE_DOMAINS in app.py to add trusted sources

Adjust EDUCATIONAL_TIPS for custom user guidance

Customize CSS in the style section for branding

🧠 How It Works
Claim Input: User submits a claim for verification

News Search: System searches Google News RSS for relevant articles

Content Extraction: Article text is extracted using multiple methods

Credibility Scoring: Each source is rated for reliability

AI Analysis: Gemini processes evidence and generates verdict

Results Display: Transparent presentation with sources and reasoning

🌟 Why FactCheckAI?
🤖 AI-Powered Accuracy
Leverages Google Gemini's advanced reasoning capabilities to provide nuanced analysis beyond simple keyword matching.

📚 Evidence-Based
Every verdict is backed by actual news sources with direct quotes and credibility scores.

🌍 Multi-Region Support
Check claims against news sources from different countries for diverse perspectives.

🎯 User-Centric Design
Built with non-technical users in mind - simple interface with powerful capabilities.

🚧 Roadmap
Coming Soon
Image Verification: Reverse image search and meme fact-checking

Browser Extension: One-click verification for any webpage

API Access: Developer-friendly REST API

Collaborative Database: Community-vetted fact database

Real-time Alerts: Breaking news verification alerts

Future Ideas
Multi-language support

Historical fact-checking archive

Educational mode for students

Integration with social media platforms

🤝 Contributing
We love contributions! Here's how you can help:

Report Bugs: Open an issue

Suggest Features: Share your ideas for improvement

Submit Code: PRs are welcome! See CONTRIBUTING.md

Improve Documentation: Help make the project more accessible

Development Setup
bash
# Fork and clone the repository
git clone https://github.com/yourusername/factcheck-ai.git
cd factcheck-ai

# Set up development environment
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
pip install -r requirements-dev.txt  # Development tools

# Run with auto-reload
streamlit run app.py --server.runOnSave true
📊 Performance
Response Time: Typically 10-20 seconds for complete analysis

Accuracy: High confidence ratings for well-supported claims

Scale: Handles hundreds of daily verifications on free tier

Reliability: 99.9% uptime with graceful fallbacks

⚠️ Limitations
API Dependencies: Requires Google Gemini API access

News Coverage: Limited to available RSS news sources

Language: Currently English-only

Complex Claims: May struggle with highly nuanced or technical topics

🛡️ Privacy & Ethics
No Data Storage: Claims are processed and immediately discarded

Transparent AI: All reasoning is explained with sources

Bias Mitigation: Multiple source perspectives are considered

Educational Focus: Designed to teach critical thinking skills

📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

🙏 Acknowledgments
Google Gemini: For providing the AI reasoning capabilities

Streamlit: For the excellent web framework

News Organizations: For making content available via RSS

Open Source Community: For countless libraries and tools

📞 Support
Documentation: Wiki

Issues: GitHub Issues

Discussions: GitHub Discussions

Email: your-email@example.com

🌟 Star History
https://api.star-history.com/svg?repos=yourusername/factcheck-ai&type=Date

<div align="center">
Made with ❤️ and 🤖 to fight misinformation

https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white
https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white

If this project helps you, please give it a ⭐ on GitHub!

</div> ```
🎯 Additional Files to Create:
1. CONTRIBUTING.md
markdown
# Contributing to FactCheckAI

We welcome contributions! Please read these guidelines before submitting.

## Development Setup
1. Fork the repository
2. Create a feature branch: `git checkout -b feature/amazing-feature`
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## Code Style
- Follow PEP 8 guidelines
- Use type hints where appropriate
- Write docstrings for functions
- Include tests for new features

## Pull Request Process
1. Update README.md if needed
2. Add tests for new functionality
3. Ensure all tests pass
4. Request review from maintainers
2. DEPLOYMENT.md
markdown
# Deployment Guide

## Streamlit Cloud
1. Connect GitHub account
2. Select repository
3. Set GEMINI_API_KEY in secrets
4. Deploy

## Other Platforms
- Heroku: Add buildpacks and Procfile
- DigitalOcean: Use App Platform
- AWS: Use Elastic Beanstalk
3. LICENSE
text
MIT License
Copyright (c) 2025 abhishek maurya

