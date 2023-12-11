# Active Subdomain Finder
This is a bash script that runs subfinder, then goes through the list of subdomains that it generates to try to find ones that are active.

I'm aware that subfinder already has an `-active` flag, but in my experience, it doesn't really work; it often returns no active subdomains, even though plenty are still in use.

## Requirements
1. Your computer must have `subfinder` installed.
2. Your computer must have `curl` installed.
3. For the text banner, your computer must also have `figlet` installed.

## How to Run
To run the script, do `bash active-subdomain-finder <base domain>`.

You could also do `chmod +x active-subdomain-finder` and then do `./active-subdomain-finder <base domain>`.

For example, `./active-subdomain-finder example.com` would try to find all subdomains for `example.com` and then check each one to see if they're active.
