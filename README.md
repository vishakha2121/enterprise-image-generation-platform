# 🎨 Enterprise Image Generation Platform

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![React](https://img.shields.io/badge/React-18.0+-61DAFB.svg)](https://reactjs.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.104+-009688.svg)](https://fastapi.tiangolo.com/)
[![Tailwind](https://img.shields.io/badge/Tailwind-3.3-38B2AC.svg)](https://tailwindcss.com/)
[![SQLite](https://img.shields.io/badge/SQLite-3.0-003B57.svg)](https://www.sqlite.org/)
[![Gemini](https://img.shields.io/badge/Gemini-API-4285F4.svg)](https://ai.google.dev/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)
[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)

> An AI-powered enterprise image generation platform for creating custom brand visuals, product designs, and industrial visualizations using Google's Gemini API.

## 📸 Project Showcase

<p align="center">
  <img src="docs/images/dashboard-preview.png" alt="Dashboard Preview" width="800"/>
  <br/>
  <em>Modern, intuitive interface for enterprise image generation</em>
</p>

---

## 📋 Table of Contents

- [🎯 Overview](#-overview)
- [✨ Features](#-features)
- [🚀 Quick Start](#-quick-start)
- [📁 Project Structure](#-project-structure)
- [🛠️ Tech Stack](#️-tech-stack)
- [📊 Database Schema](#-database-schema)
- [🔌 API Endpoints](#-api-endpoints)
- [🎨 UI Components](#-ui-components)
- [📱 Screenshots](#-screenshots)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)
- [🙏 Acknowledgments](#-acknowledgments)

---

## 🎯 Overview

The **Enterprise Image Generation Platform** is a comprehensive solution designed to revolutionize how businesses create visual content. By leveraging Google's powerful Gemini AI, this platform enables teams to generate high-quality, brand-consistent images without requiring expensive GPU infrastructure.

### 🎯 Why This Platform?

| Challenge | Solution |
|-----------|----------|
| 💰 High GPU Costs | Uses Gemini API - no GPU needed |
| 🎨 Inconsistent Branding | Brand style management system |
| ⏰ Slow Design Process | AI-powered rapid generation |
| 👥 Team Collaboration | Project-based organization |
| 🔒 Security Concerns | Enterprise-grade authentication |
| 📈 Scaling Issues | Scalable architecture |

### 👥 Who Is This For?

- **Marketing Teams**: Create campaign visuals instantly
- **Product Designers**: Rapid prototyping and iteration
- **Creative Agencies**: Client presentations and mockups
- **E-commerce Managers**: Product image generation
- **Brand Managers**: Maintain visual consistency
- **Content Creators**: Generate unique visuals for content

---

## ✨ Features

### 🎨 Core Features

#### 1. AI Image Generation
- **Text-to-Image**: Generate images from detailed prompts
- **Style Transfer**: Apply custom brand styles
- **Batch Generation**: Create multiple variations
- **Prompt Enhancement**: AI-powered prompt optimization
- **Negative Prompts**: Exclude unwanted elements

#### 2. Brand Style Management
- **Custom Styles**: Create and save brand-specific styles
- **Color Palettes**: Define brand color schemes
- **Style Templates**: Pre-designed templates
- **Style Preview**: See styles before applying
- **Style Sharing**: Share styles across team

#### 3. Project Management
- **Project Organization**: Organize by projects
- **Version Control**: Track image versions
- **Team Collaboration**: Share projects
- **Asset Management**: Centralized repository
- **Export Options**: Multiple formats supported

#### 4. User Experience
- **Modern UI**: Clean, intuitive interface
- **Dark/Light Mode**: Theme preferences
- **Responsive Design**: Works on all devices
- **Real-time Preview**: See results instantly
- **Loading Animations**: Engaging user experience

#### 5. Enterprise Features
- **User Authentication**: Secure JWT-based auth
- **Role Management**: Admin, User, Viewer roles
- **Activity Logging**: Track all actions
- **Analytics Dashboard**: Usage metrics
- **API Rate Limiting**: Prevent abuse

### 🔮 Future Features
- Integration with Figma, Adobe Suite
- Real-time collaboration
- Advanced fine-tuning
- Mobile application
- AI image enhancement
- Video generation

---

## 🚀 Quick Start

### 📋 Prerequisites

Before you begin, ensure you have the following installed:

```bash
# Check Python version
python --version  # Should be 3.8 or higher

# Check Node.js version
node --version   # Should be 16.0 or higher

# Check npm version
npm --version    # Should be 7.0 or higher

# Check Git version
git --version    # Should be 2.0 or higher

# Clone the repository
git clone https://github.com/yourusername/enterprise-image-generation-platform.git
cd enterprise-image-generation-platform

# Or use SSH
git clone git@github.com:yourusername/enterprise-image-generation-platform.git
cd enterprise-image-generation-platform

# Navigate to backend
cd backend

# Create virtual environment
python -m venv venv

# Activate virtual environment
# On Windows:
venv\Scripts\activate
# On Mac/Linux:
source venv/bin/activate

# Install dependencies
pip install --upgrade pip
pip install -r requirements.txt

# Create .env file
cp .env.example .env

# Edit .env with your configurations
# Add your GEMINI_API_KEY here

# Initialize database
python init_db.py

# Run migrations
alembic upgrade head

# Seed demo data (optional)
python scripts/seed_data.py

# Open new terminal, navigate to frontend
cd frontend

# Install dependencies
npm install

# Create .env file
cp .env.example .env

# Update API URL if needed
# REACT_APP_API_URL=http://localhost:8000/api