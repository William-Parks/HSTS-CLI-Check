# HSTS Header Checker

**HSTS Header Checker** is a simple Bash tool that checks a list of websites for the presence of the HTTP Strict Transport Security (HSTS) header. It helps you quickly audit multiple domains for HSTS implementation, which is an important security best practice.

---

## Features

- **Interactive**: Prompts you for a file containing a list of websites to check.
- **Automated Scanning**: Scans each website for the `Strict-Transport-Security` header using `curl`.
- **Clear Reporting**: Clearly reports whether the HSTS header is found for each site.
- **Debug Support**: If the HSTS header is missing, displays a sample of the raw HTTP response headers for troubleshooting.
- **Flexible Output**: Supports a `-o` flag to save the output to a file while also displaying it in the terminal.
- **Help Option**: Includes a `-h` flag for a helpful usage guide.

---

## Usage

./check_hsts.sh [-o outputfile] [-h]


- **Run the script** and follow the prompt to specify your website list file (one domain per line).
- Use `-o outputfile` to **save results to a file** (output will still be shown in the terminal).
- Use `-h` to **display the help message**.

---

## Example

./check_hsts.sh -o results.txt


---

## Who is this for?

This tool is ideal for sysadmins, developers, and security professionals who want a quick way to verify HSTS deployment across many domains.

---

## License

MIT License
