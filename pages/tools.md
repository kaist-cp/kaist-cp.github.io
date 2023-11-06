---
title: Tools
description: 장인은 도구를 가린다.
background: /assets/images/kaist.jpg
permalink: /tools
---

## Services

- Calendar: <https://calendar.google.com/>
- Email: <https://mail.google.com/>
- Drive
  + Google: <https://drive.google.com/>
  + Nextcloud: <https://nextcloud.fearless.systems/>
- Chat: <https://chat.fearless.systems/>
- Git repositories
  + GitLab: <https://git.fearless.systems/>
  + GitHub: <https://github.com/kaist-cp/>
- Development machines: <https://dev.fearless.systems/>
  + The `/home/$USER/local-home` directory is local/single SSD (not remote/replicated HDD like home's other directories).
    *WARNING*: this directory is more likely to be lost, e.g., due to media failure.
  + The `/home/$USER/share` directory is shared to the lab members at `/home/_share/$USER`.
  + The `/home/$USER/share/www` directory is served at <https://public.fearless.systems/$USER>.
    *WARNING*: it's open to the internet.
- VPNs
  + Rack (server room): <https://rack.fearless.systems/>
  + Office: <https://office.fearless.systems/>
- Internal document: <https://git.fearless.systems/kaist-cp/infra-internal>
- Courses
  + CS431: <https://github.com/kaist-cp/cs431/>
  + CS420: <https://github.com/kaist-cp/cs420/>
  + CS220: <https://github.com/kaist-cp/cs220/>

## Onboarding

- Send an email from your `{firstname}.{lastname}@kaist.ac.kr` account to Jeehoon (`jeehoon.kang@kaist.ac.kr`).

- Account (Google Workspace): receive your `{firstname}.{lastname}@cp.kaist.ac.kr` Google Workspace account from Jeehoon.
  You will use this account for all the web services (except for GitHub).

- [Calendar (Google)](https://calendar.google.com):
  Manage your schedule here.
  If you want to have a meeting, just create a schedule, write down agenda, and directly invite people.

- [Email (Google)](https://mail.google.com)

    + Write [proper formal emails](https://www.wikihow.com/Write-a-Formal-Email). Do not heavily markup emails.

    + Check both `{firstname}.{lastname}@kaist.ac.kr` and `{firstname}.{lastname}@cp.kaist.ac.kr` email accounts.
      FYI, Jeehoon forwards emails from `{firstname}.{lastname}@kaist.ac.kr` to `{firstname}.{lastname}@cp.kaist.ac.kr` and check emails in Gmail.

- [Drive, Docs, Spreadsheet, Slide, Form (Google)](https://drive.google.com):
  Put all project-related files to shared Google Drive.

- [Drive (Nextcloud)](https://nextcloud.fearless.systems/)

  I recommend you to set up an "external storage" to your home directory.
  In [here](https://nextcloud.fearless.systems/settings/user/externalstorages), add an SFTP connection with the following configuration:

    + Authentication: username and password

    + Host: `10.30.0.2:2200`

    + Root: `/kaist-cp-home/{google-workspace-id}`

    + Username: `{google-workspace-id}`

    + Password: `{google-workspace-password}`

- [Chat (Zulip)](https://chat.fearless.systems)

    + First things first, say hi in [this topic](https://chat.fearless.systems/#narrow/stream/112-general/topic/.EC.86.8C.EA.B0.9C).

    + It is our primary method of communication.

- Git repositories

    + [GitLab](https://git.fearless.systems): browse projects to see what's interesting.

    + GitHub: we're at the [`kaist-cp` organization](https://github.com/kaist-cp).
      Display your real name in your public profile (Settings > Profile > Name).
      We prefer GitLab to GitHub, though.

    + If you want to create a new organization or repository, ask Jeehoon.

    + Configure email notifications for mentions and issue/PR/MR comments.

- [Website]({{ site.baseurl }})

    + Fork [the website repository](https://github.com/kaist-cp/kaist-cp.github.io) and clone it.

    + Install dependencies and run a local server to test as follows:

      ```bash
      # Make sure Ruby is installed.
      $ bundle exec jekyll serve
      ```

    + Add your information (e.g., name, status, GitHub ID) to `people.yml`.

    + Create a new file `{firstname}.{lastname}.md` under the directory `_people/`. See `_people/jeehoon.kang.md` for reference.
      Your website is `https://cp.kaist.ac.kr/{firstname}.{lastname}`.

    + Commit your changes and send a PR.

    + Keep maintaining your website.

- Development

    + Learn VSCode. 
    
      If you insist on 적폐 editors like Vim or Emacs, I won't fight with you. But keep in your mind that the winner of the editor war---vim vs emacs---is vs(code).

    + Learn Git. 
    
      Here are good tutorials from [Atlassian](https://www.atlassian.com/git/tutorials) and [GitHub](https://lab.github.com/).

    + Learn SSH.

        * Generate your ed25519 SSH key: <https://www.ssh.com/academy/ssh/keygen>.

        * Authorize the key in servers: <https://www.ssh.com/academy/ssh/copy-id>. From now on, you must never write down password every time.

        * Configure your local SSH config: <https://linuxize.com/post/using-the-ssh-config-file/>

        * Use `ssh-agent`.

    + Study [The Missing Semester of Your CS Education](https://missing.csail.mit.edu/) ([Korean translation](https://missing-semester-kr.github.io/)), except for "Editors (Vim)".
      Again, please use VSCode.

    + Use the development machines as [described here](#services).
