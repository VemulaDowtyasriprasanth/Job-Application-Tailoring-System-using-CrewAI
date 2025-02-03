```markdown
# Job Application Tailoring System using CrewAI

## Description
This project implements a multi-agent system using CrewAI to automate and enhance the job application process. The system analyzes job postings, tailors resumes, and prepares interview materials using AI agents working collaboratively.

## Features
- Job posting analysis and requirement extraction
- Professional profile compilation
- Resume tailoring based on job requirements
- Interview preparation materials generation
- Multi-agent collaboration system
- Automated document generation

## Prerequisites
- Python 3.x
- OpenAI API key
- Serper API key

## Installation
1. Clone the repository:
```bash
git clone [repository-url]
```

2. Install required packages:
```bash
pip install crewai==0.28.8 crewai_tools==0.1.6 langchain_community==0.0.29
```

## Project Structure
- `main.py`: Main script containing the implementation
- `utils.py`: Utility functions for API key management
- `fake_resume.md`: Sample resume template
- Generated files:
  - `tailored_resume.md`: Customized resume output
  - `interview_materials.md`: Generated interview preparation materials

## Agents
1. **Tech Job Researcher**: Analyzes job postings and requirements
2. **Personal Profiler**: Researches and profiles job applicants
3. **Resume Strategist**: Tailors resumes to match job requirements
4. **Interview Preparer**: Creates interview questions and talking points

## Usage
1. Set up your environment variables:
```python
os.environ["OPENAI_API_KEY"] = "your-api-key"
os.environ["SERPER_API_KEY"] = "your-serper-api-key"
```

2. Run the system with your inputs:
```python
job_application_inputs = {
    'job_posting_url': 'your-job-posting-url',
    'github_url': 'your-github-url',
    'personal_writeup': 'your-personal-description'
}

result = job_application_crew.kickoff(inputs=job_application_inputs)
```

## Tools Used
- CrewAI
- OpenAI GPT Models
- Serper API
- File Reading Tools
- Web Scraping Tools
- Semantic Search Tools

## Configuration
- Default LLM: GPT-3.5-turbo
- Configurable to use GPT-4-turbo when running locally
- Customizable agent roles and tasks

## Output
The system generates two main files:
1. `tailored_resume.md`: A customized resume matching the job requirements
2. `interview_materials.md`: Interview preparation materials including questions and talking points

## Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

## License
[Your chosen license]

## Acknowledgments
- CrewAI framework
- DeepLearning.AI
- [Other acknowledgments]


