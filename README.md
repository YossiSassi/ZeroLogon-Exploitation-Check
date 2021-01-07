Script to automate Checks for potential exploitation of CVE-2020-1472 (aka ZeroLogon) in the domain.
This is a *very* "quick and dirty" script that automates some of the leading artifects in determining an actual exploitation of CVE-2020-1472, compiled from multiple blogs.
Ideally, the 2nd check (for events from Security & System event logs) can be done from a SIEM/Syslog/Event collector, which keeps events far enough back to detect such exploits.
Note that if netlogon logs were not enabled in the environment, and DC logs were overwritten by newer events, an exploitation could have happened and would not be noticed by the remaining artifacts in the environment checked.
Can also run this script to detect future exploitations, although other methods exist, from NEtwork/EPP etc (read more on netlogon debug before turning it On for a long period of time).
