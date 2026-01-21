# Parth_Ids568-ML-Op




# MLOps Environment Setup - Milestone 0

[![CI](https://github.com/ParthPatel0226/Parth_Ids568-ML-Ops/actions/workflows/Ci.yml/badge.svg)](https://github.com/ParthPatel0226/Parth_Ids568-ML-Ops/actions/workflows/Ci.yml)

## Project Overview
This repository demonstrates reproducible environment setup and CI/CD automation for MLOps workflows, establishing the foundation for reliable machine learning systems.

## Setup Instructions

### Prerequisites
- Python 3.10 or higher
- Git

### Installation Steps

1. **Clone the repository**
```bash
   git clone https://github.com/ParthPatel0226/Parth_Ids568-ML-Ops.git
   cd Parth_Ids568-ML-Ops
```

2. **Create and activate virtual environment**
```bash
   python -m venv venv
   source venv/bin/activate  # Windows: venv\Scripts\activate
```

3. **Install dependencies**
```bash
   pip install --upgrade pip
   pip install -r requirements.txt
```

4. **Run tests**
```bash
   pytest tests/ -v
```

## Environment Reproducibility & ML Lifecycle

Environment reproducibility forms the foundation of reliable MLOps systems. By pinning exact dependency versions, we ensure models trained during development produce identical results in production, preventing costly deployment failures. This practice supports the entire ML lifecycle: consistent data preprocessing eliminates training-serving skew, deterministic model behavior enables accurate A/B testing, and reproducible environments facilitate seamless team collaboration. When dependencies drift between environments, models can silently degrade or fail completely. Our implementation uses exact version pinning (numpy==2.4.1) rather than version ranges, automated CI testing validates environment consistency across clean installations, and comprehensive documentation enables anyone to recreate our setup identically. This directly impacts deployment success—reproducible environments mean predictable model behavior, faster debugging when issues arise, and confident production releases. By establishing these engineering practices from the start, we build the foundation for scalable, maintainable machine learning systems.

## Project Structure
```
├── .github/workflows/    # CI/CD automation
├── src/                  # Source code
├── tests/                # Test suite
├── requirements.txt      # Pinned dependencies
└── README.md            # Documentation
```

## Technologies Used
- **Python 3.14** - Primary language
- **pytest 8.0.0** - Testing framework
- **NumPy 2.4.1** - Numerical computing
- **Pandas 2.2.0** - Data manipulation
- **GitHub Actions** - CI/CD automation

## Continuous Integration
This project uses GitHub Actions for automated testing. Every push triggers tests in a clean environment to verify reproducibility. The CI badge above shows current build status.

## Author
Parth Patel - MS in MIS, University of Illinois Chicago
