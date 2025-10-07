# CICD Demo - Security Enhanced Spring Boot Application

[![Java CI with Maven](https://github.com/Tshewangdorji7257/CICD-Demo/actions/workflows/maven.yml/badge.svg)](https://github.com/Tshewangdorji7257/CICD-Demo/actions/workflows/maven.yml)
[![SonarCloud Security Analysis](https://github.com/Tshewangdorji7257/CICD-Demo/actions/workflows/sonarcloud.yml/badge.svg)](https://github.com/Tshewangdorji7257/CICD-Demo/actions/workflows/sonarcloud.yml)
[![Enhanced Security Pipeline](https://github.com/Tshewangdorji7257/CICD-Demo/actions/workflows/enhanced-security.yml/badge.svg)](https://github.com/Tshewangdorji7257/CICD-Demo/actions/workflows/enhanced-security.yml)

## Overview

This project demonstrates a comprehensive **CI/CD security pipeline** integrating **Static Application Security Testing (SAST)** tools as part of **SWE302 Practical 4 & 4a**.

### 🔐 Security Features
- **Snyk**: Dependency vulnerability scanning and code security analysis
- **SonarCloud**: Comprehensive SAST with quality gates
- **GitHub Actions**: Automated security workflows
- **JaCoCo**: Code coverage reporting
- **SARIF Integration**: Security results in GitHub Security tab

### 🏗️ Tech Stack
- **Framework**: Spring Boot 3.1.2
- **Language**: Java 17
- **Build Tool**: Maven
- **Testing**: JUnit 5 + Spring Boot Test
- **Security**: Snyk + SonarCloud
- **CI/CD**: GitHub Actions

## 🚀 Quick Start

### Prerequisites
- Java 17+
- Maven 3.6+
- Git

### Local Development
```bash
# Clone the repository
git clone https://github.com/Tshewangdorji7257/CICD-Demo.git
cd CICD-Demo

# Build and test
mvn clean verify

# Run the application
mvn spring-boot:run
```

### API Endpoints
- `GET /` - Health check
- `GET /version` - Application version
- `GET /nations` - Random nation data
- `GET /currencies` - Random currency data

## 🔒 Security Implementation

This project implements enterprise-grade security practices:

### Security Scanning Tools
- **Snyk**: Identifies vulnerabilities in dependencies and source code
- **SonarCloud**: Performs comprehensive SAST analysis
- **GitHub Security**: Automated security advisories and dependency updates

### Quality Gates
- Zero tolerance for high/critical security vulnerabilities
- Mandatory security hotspot reviews
- Code coverage thresholds enforced
- Quality metrics tracked over time

### Automated Workflows
1. **Pull Request Scanning**: Every PR is automatically scanned
2. **Scheduled Security Checks**: Weekly vulnerability assessments
3. **Production Monitoring**: Continuous dependency monitoring
4. **Security Alerts**: Automated notifications for critical issues

## 📊 Security Dashboard

### GitHub Security Tab
All security scan results are integrated into GitHub's Security tab:
- **Code Scanning**: View SAST findings from SonarCloud and Snyk
- **Dependency Review**: Track vulnerable dependencies
- **Security Advisories**: Automated vulnerability notifications

### SonarCloud Dashboard
- **Project URL**: [SonarCloud Project](https://sonarcloud.io/project/overview?id=Tshewangdorji7257_cicd-demo)
- **Quality Gates**: Enforced security and quality standards
- **Security Hotspots**: Manual review required items
- **Coverage Reports**: Code coverage tracking

## 🛠️ Configuration

### Required GitHub Secrets
Set these in `Settings` → `Secrets and variables` → `Actions`:
- `SNYK_TOKEN`: Snyk API token
- `SONAR_TOKEN`: SonarCloud authentication token
- `SONAR_ORGANIZATION`: SonarCloud organization key

### Configuration Files
- `.snyk`: Snyk vulnerability scanning configuration
- `sonar-project.properties`: SonarCloud analysis settings
- `.github/workflows/`: Automated security workflows

## 📈 Security Metrics

Current security status:
- **Vulnerabilities**: 0 Critical, 0 High
- **Security Rating**: A
- **Coverage**: >80%
- **Quality Gate**: ✅ Passing

## 🔍 Security Best Practices Demonstrated

1. **Shift Left Security**: Integration early in development process
2. **Automated Scanning**: No manual intervention required
3. **Quality Gates**: Prevent insecure code from deployment
4. **Continuous Monitoring**: Ongoing vulnerability assessment
5. **Compliance Tracking**: Security metrics and reporting

## 📚 Documentation

- **Security Setup**: [SECURITY.md](./SECURITY.md) - Comprehensive security implementation guide
- **API Documentation**: Available at `/swagger-ui` when running locally
- **Test Reports**: Generated in `target/site/` after running tests

## 🎯 Learning Objectives (SWE302)

This project demonstrates mastery of:
- ✅ SAST integration with development workflows
- ✅ Vulnerability management and remediation
- ✅ Quality gate implementation and enforcement
- ✅ Security metrics collection and reporting
- ✅ DevSecOps best practices

## 📝 Practical Requirements Met

**Practical 4 - Snyk Integration**:
- ✅ Snyk account setup and configuration
- ✅ GitHub Actions integration
- ✅ Vulnerability scanning automation
- ✅ SARIF report generation

**Practical 4a - SonarCloud Integration**:
- ✅ SonarCloud account and project setup
- ✅ Quality gates configuration
- ✅ Security analysis automation
- ✅ Continuous monitoring implementation

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Ensure all security scans pass
4. Submit a pull request

All contributions must pass security quality gates before merging.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

**Security Status**: 🟢 Secure | **Build Status**: ✅ Passing | **Coverage**: 📊 >80%