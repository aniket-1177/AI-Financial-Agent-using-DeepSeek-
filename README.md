# AI Financial Agent using DeepSeek

##  Overview

DeepSeek AI Financial Agent is a sophisticated market analysis tool that harnesses the power of DeepSeek LLM and multi-agent architecture. Built using the Phi framework, it provides comprehensive financial insights, market analysis, and stock recommendations through both CLI and an interactive web interface.

##  Features

-  Stock market analysis
-  Latest market news integration
-  Analyst recommendations tracking
-  Dual interface: CLI and Web UI
-  Multi-agent architecture for enhanced accuracy

##  Quick Start

### Prerequisites

```bash
Python 3.9+
pip (Python package installer)
```

### Installation

1. Clone the repository:
```bash
git clone https://github.com/aniket-1177 AI-Financial-Agent-using-DeepSeek-.git
cd deepseek-financial-agent
```

2. Create and activate virtual environment:
```bash
# Create virtual environment
python -m venv venv

# Activate virtual environment
venv\Scripts\activate # For Windows
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Set up environment variables:
```bash
# Create .env file
touch .env

# Add the following to your .env file:
PHI_API_KEY=your_phi_api_key_here
GROQ_API_KEY=your_groq_api_key_here
```

##  Usage

### CLI Version (Terminal)

Run the CLI version for quick financial analysis:

```bash
python cli_agent.py
```

Example command:
```bash
"Summarize analyst recommendation and share the latest news for NVDA"
```

### Web Interface Setup

1. Create an account at [Phidata](https://phidata.com)
2. Navigate to the Playground section in your Phidata dashboard
3. Launch the local server:
```bash
python playground_agent.py
```
4. In the Phidata Playground:
   - Configure the endpoint to `localhost:7777`
   - Connect to your local instance
   - Start interacting with the AI agent

##  Architecture

DeepSeek AI Financial Agent utilizes a multi-agent architecture:

1. **Finance Agent**: Handles financial data processing and analysis
   - Stock price tracking
   - Analyst recommendations
   - Company fundamentals
   - Market news aggregation

2. **Web Search Agent**: Provides additional context and real-time information
   - Web scraping capabilities
   - News verification
   - Market sentiment analysis

##  Technical Stack

- **Framework**: Phidata
- **LLM**: DeepSeek (deepseek-r1-distill-llama-70b)
- **Data Sources**: 
  - YFinance
  - DuckDuckGo
- **UI**: Phidata Playground
