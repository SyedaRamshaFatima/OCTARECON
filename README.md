OCTARECON

OCTARECON is a modular, Python-based command-line tool developed on Kali Linux to streamline network reconnaissance and information gathering. Tailored for cybersecurity professionals, it combines multiple essential features into a single, user-friendly CLI interface for efficient domain and IP analysis.

Features:

Each feature in OCTARECON is implemented as an independent module for flexibility and scalability:

Tool	Description:

IP Lookup (I)	Resolves a domain to its IP address using DNS resolution.
GeoIP Lookup (G)	Fetches geographic details (country, city, ISP) for an IP address.
IP Netblock Analysis (N)	Identifies the network block and ownership of an IP.
CMS Detection (C)	Detects CMS platforms like WordPress, Joomla, or Drupal used by the target website.
Subdomain Enumeration (S)	Discovers subdomains related to a domain for broader surface mapping.
Whois Lookup (W)	Retrieves registration data including domain owner and expiry info.
SSL Information (L)	Extracts SSL/TLS certificate details for evaluating HTTPS configuration.
Email Harvesting (E)	Collects publicly exposed email addresses related to the target domain.
Run All (A)	Executes all tools in one go for a full analysis.

Technical Overview:

Platform: Kali Linux (tested and developed)
Language: Python
Interface: Command-line (CLI)
Modular Architecture: Each tool is implemented in a separate file under the tools directory.
Logging: Outputs are saved to both the console and a finalresult.txt file.
Progress Tracking: Uses tqdm to show progress bars for better user feedback.
Error Handling: Includes input validation and exception handling to prevent crashes.

How It Works:

Menu Display: Users are greeted with an ASCII art banner and a list of tool options.
Input Prompt: Enter the domain name and select desired tools via letter codes (e.g., I, C, W).
Execution: Selected tools are run one-by-one or all together if A is selected.
Logging: Output is displayed on the terminal and written to finalresult.txt.
Timing: Total execution time is calculated and shown.

Future Improvements:

Add DNS enumeration and vulnerability scanners.
Build a GUI for ease of use.
Enable parallel execution to improve speed.
Integrate threat intelligence APIs for real-time insights.
