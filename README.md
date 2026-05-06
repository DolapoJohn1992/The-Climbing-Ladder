The Climbing Ladder: Privilege Escalation
## Project Overview
This project demonstrates Linux privilege escalation techniques by transitioning from a limited user to root access. The primary focus was identifying misconfigured binary permissions and leveraging the `find` utility to establish a persistent root shell.

## Technical Stack
* **Operating System:** Ubuntu Linux
* **Tools:** Bash, Git/GitHub, `find` binary
* **Environment:** VirtualBox, VS Code

## Project Phases
1. **Initial Access:** Logged into the system as `limited_user`.
2. **Vulnerability Discovery:** Audited SUID binaries and discovered that the `find` command could be run with root privileges without a password.
3. **Exploitation:** Used the `-exec` flag within `find` to execute a shell command, successfully spawning a root shell.
4. **Persistence:** Created a root-owned SUID copy of bash at `/tmp/rootbash` to maintain administrative access.

## Portfolio Artifacts
* **escalation_path.txt**: A detailed log of the methodology and commands used to achieve root access.# The-Climbing-Ladder
