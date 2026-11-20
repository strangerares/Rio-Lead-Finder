
# Rio Lead Finder

An automated lead discovery and qualification system for Rio Private Driver.

The purpose of this project is to identify potential business partners and customers in the international travel industry, particularly in the United States and Canada.

## Project objectives

Discover and qualify:

- Travel agencies specialising in Brazil and South America.
- Independent travel advisors.
- Luxury travel planners.
- International tour operators.
- Hotels and accommodation businesses.
- Destination wedding and event planners.
- Relevant public travel discussions and opportunities.

## Main features

### 1. Lead Discovery
Search publicly available information to identify relevant businesses and potential opportunities.

### 2. AI Lead Qualification
Use Google's Gemini API to analyse discovered businesses and assign a relevance score from 0 to 100.

### 3. Lead Management
Store qualified leads in Supabase, including:

- Company name
- Website
- Country
- Business category
- Public business contact information
- Description and specialisation
- Lead relevance score
- Discovery source
- Discovery date
- Outreach status

### 4. Outreach Assistant
Generate personalised partnership proposals and business emails for human review and approval.

### 5. Reporting
Track discovered leads, qualified prospects, contacted businesses and responses.

## Technology stack

- Python
- GitHub
- GitHub Actions
- Supabase
- Google Gemini API
- Search APIs

## Project structure

```text
rio-lead-finder/
│
├── src/
│   ├── discovery/
│   ├── qualification/
│   ├── outreach/
│   ├── database/
│   └── main.py
│
├── tests/
│
├── config/
│
├── data/
│
├── .github/
│   └── workflows/
│
├── .env.example
├── .gitignore
├── requirements.txt
└── README.md
```

## Installation

Clone the repository:

```bash
git clone YOUR_REPOSITORY_URL
cd rio-lead-finder
```

Create a virtual environment:

```bash
python -m venv .venv
```

Activate it:

Windows:

```bash
.venv\Scripts\activate
```

Linux / macOS:

```bash
source .venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Configure environment variables using `.env.example` as a template.

## Environment variables

The application may require:

- GEMINI_API_KEY
- SUPABASE_URL
- SUPABASE_KEY
- SEARCH_API_KEY

Never commit API keys, passwords or other credentials to GitHub.

## Automation

GitHub Actions will eventually run the discovery process automatically on a scheduled basis.

## Data collection and compliance

- Collect information from publicly accessible sources.
- Respect website terms of service and robots.txt where applicable.
- Follow applicable privacy and data protection laws.
- Store only relevant business information.
- Avoid collecting private browsing information.
- Require human approval before sending outreach messages.
- Respect opt-out and unsubscribe requests.

## Development roadmap

- [ ] Initial project structure
- [ ] Search and discovery module
- [ ] Business website extraction
- [ ] Gemini lead qualification
- [ ] Supabase integration
- [ ] Duplicate lead detection
- [ ] Lead scoring system
- [ ] Personalised outreach generation
- [ ] Lead management dashboard
- [ ] Automated GitHub Actions execution
- [ ] Performance reporting

## Project

Developed for Rio Private Driver.

Website: https://rioprivatedriver.com/
# Rio-Lead-Finder
