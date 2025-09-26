Initial Setup:

Create a new GitHub repository with a README file

Access GitHub Codespaces through the repository

Select a 4-core machine configuration for better performance

Launch a blank Codespaces template

Server Configuration:
The video guides through installing Docker and setting up the environment using these commands:

sudo su (gain root access)

sudo apt update (update package list)

sudo apt install docker.io docker-compose (install Docker components)

Create a windows10.yml Docker Compose file with Windows configuration

Run sudo docker compose -f windows10.yml up to launch the Windows container

Access Method:

The Windows RDP server becomes accessible through GitHub's port forwarding feature

Users can connect via web browser to access a full Windows desktop environment

The setup provides admin/root access to the Windows instance

Technical Reality and Limitations
Free Usage Constraints:
GitHub provides 120 core hours monthly for free accounts, which equals about 60 hours on a 2-core machine or 30 hours on a 4-core machine. This isn't truly "unlimited 24/7" access as the video title suggests.

Performance Considerations:
The video claims to show disk space and internet speed testing, but actual performance will depend on GitHub's infrastructure and current load. Codespaces run on GitHub's cloud VMs with varying specifications.

Security and Compliance Concerns
Potential Security Risks:
Running Docker-in-Docker configurations and publicly exposing ports can create security vulnerabilities. Research shows that malicious actors can abuse GitHub Codespaces for hosting malware by exploiting the port forwarding feature.

Terms of Service:
Using GitHub Codespaces primarily as a free VPS/RDP server rather than for legitimate development work may violate GitHub's terms of service. The platform is designed for software development, not general computing or server hosting.

Resource Abuse:
The method essentially uses GitHub's development infrastructure for purposes beyond its intended use, which could lead to account suspension if detected.

Legitimate Alternatives
For genuine development needs, GitHub Codespaces is excellent for its intended purpose - providing consistent development environments. For free RDP access, consider legitimate providers that offer 30-day free trials with proper terms of service compliance.

The video technique works temporarily but carries significant risks regarding account security, terms of service violations, and sustainability for long-term use.