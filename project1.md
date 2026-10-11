Final_STIGs
===========

- **Class:** CSCI 301 - Survey of Programming Languages
- **Grade:** A (course grade)
- **Language(s):** Bash
- **Source Code Repository:** [CSCI301-Final-STIGs](https://github.com/afrycz/CSCI301-Final-STIGs)

Project Description
-------------------

Final_STIGs is a collection of Bash scripts created to validate selected Linux security settings against DISA STIG requirements. The scripts check SSH session settings, password aging requirements, and duplicate user IDs.

The scripts display the applicable STIG requirement and the current system setting so the values can be reviewed for compliance. The duplicate UID script checks the system for accounts that share the same user ID.

How to Run the Program
----------------------

No compilation is required. The scripts are run from a Linux terminal using Bash.

Example:

```bash
bash check_password_min_days.sh
```

Some scripts may require elevated permissions to read system configuration files.

How It Works
------------

The password scripts read values from `/etc/login.defs`, while the SSH scripts read settings from `/etc/ssh/sshd_config`. The duplicate UID script uses `awk` to examine `/etc/passwd` and identify duplicate user IDs.

The two SSH validation scripts are included in the project, but they were not demonstrated in the screenshot because the Ubuntu VM used for testing did not have the OpenSSH server configuration file (`/etc/ssh/sshd_config`) installed. The scripts themselves are still included as part of the original project.

The screenshot below shows the three scripts that could be demonstrated on the Ubuntu virtual machine used for testing.

![Final_STIGs Bash scripts running on Ubuntu](images/Final_STIGS_Screenshot.png)

**Fig. 1. Final_STIGs scripts validating password aging settings and duplicate user IDs on Ubuntu.**

[Back to Portfolio](./)
