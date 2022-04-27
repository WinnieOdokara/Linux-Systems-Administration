## Linux Systems Administration

### Step 1: Ensure/Double Check Permissions on Sensitive Files

1. Permissions on `/etc/shadow` should allow only `root` read and write access.

    - Command to inspect permissions:
 &nbsp;![ ](Images/1-1-permission.jpg)&nbsp;
    - Command to set permissions (if needed):

2. Permissions on `/etc/gshadow` should allow only `root` read and write access.

    - Command to inspect permissions:
&nbsp;![ ](Images/1-2-permission.jpg)&nbsp;
    - Command to set permissions (if needed):

3. Permissions on `/etc/group` should allow `root` read and write access, and allow everyone else read access only.

    - Command to inspect permissions:
&nbsp;![ ](Images/1-3-permission.jpg)&nbsp;
    - Command to set permissions (if needed):

4. Permissions on `/etc/passwd` should allow `root` read and write access, and allow everyone else read access only.

    - Command to inspect permissions:
&nbsp;![ ](Images/1-4-permission.jpg)&nbsp;
    - Command to set permissions (if needed):

### Step 2: Create User Accounts

1. Add user accounts for `sam`, `joe`, `amy`, `sara`, and `admin`.

    - Command to add each user account (include all five users):
&nbsp;![ ](Images/creating-user-accounts.png)&nbsp;
2. Ensure that only the `admin` has general sudo access.

    - Command to add `admin` to the `sudo` group:
&nbsp;![ ](Images/admin_sudo_group.png)&nbsp;
### Step 3: Create User Group and Collaborative Folder

1. Add an `engineers` group to the system.

    - Command to add group:
&nbsp;![ ](Images/adding_engeneers-group.png)&nbsp;
2. Add users `sam`, `joe`, `amy`, and `sara` to the managed group.

    - Command to add users to `engineers` group (include all four users):
&nbsp;![ ](Images/add-users-engeneers-group.jpg)&nbsp;
3. Create a shared folder for this group at `/home/engineers`.

    - Command to create the shared folder:
&nbsp;![ ](Images/engeneers-folder.jpg)&nbsp;
4. Change ownership on the new engineers' shared folder to the `engineers` group.

    - Command to change ownership of engineer's shared folder to engineer group:
&nbsp;![ ](Images/engineers_ownership.png)&nbsp;
### Step 4: Lynis Auditing

1. Command to install Lynis:
&nbsp;![ ](Images/installing_lynis.png)&nbsp;
2. Command to see documentation and instructions:
&nbsp;![ ](Images/lynis_documentation.png)&nbsp;
3. Command to run an audit:
&nbsp;![ ](Images/lynis_audit.png)&nbsp;
4. Provide a report from the Lynis output on what can be done to harden the system.

    - Screenshot of report output:
&nbsp;![ ](Images/0-lynis-hardening.png)&nbsp;
&nbsp;![ ](Images/1-lynis_hardening.png)&nbsp;
&nbsp;![ ](Images/2-lynis_hardening.png)&nbsp;
&nbsp;![ ](Images/3-lynis_hardening.png)&nbsp;
&nbsp;![ ](Images/4-lynis_hardening.png)&nbsp;
### Bonus
1. Command to install chkrootkit:
&nbsp;![ ](Images/installing_chkrootkit.png)&nbsp;
2. Command to see documentation and instructions:
&nbsp;![ ](Images/chkrootkit_documentation.png)&nbsp;
3. Command to run expert mode:
&nbsp;![ ](Images/chkrootkit-expert-mode.jpg)&nbsp;

---

