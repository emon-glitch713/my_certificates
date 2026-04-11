# Pentesting Cheatsheets
# This repository contains essential *Nmap* and *SQLMap* commands for penetration testing and security auditing
# 1 NMAP COMMAND 
nmap -sS target.com
nmap -p- target.com
nmap -sV target.com
nmap -A target.com
nmap --script vuln target.com
nmap -o target.com 
# 2 SQLMap command 
sqlmap -u "URL" --risk=3 --level=5
sqlmap -u "URL" --batch --random-agent
sqlmap -u "target.com" --dbs
sqlmap -u "URL" -D dbname --tables
sqlmap -u "URL" -D dbname -T users --columns
sqlmap -u "URL" -D dbname -T users --dump
