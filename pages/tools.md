---
title: Tools
description: 장인은 도구를 가린다.
background: /assets/images/kaist.jpg
permalink: /tools
---

## Services

- Calendar: <https://calendar.google.com>
- Email: <https://mail.google.com>
- Drive
  + Google: <https://drive.google.com>
  + Seafile: <https://drive.fearless.systems>
- Chat
  + Zulip (Message): <https://chat.fearless.systems>
  + Jitsi Meet (Voice/Video): <https://jitsi.fearless.systems>
- Git
  + GitLab: <https://git.fearless.systems>
  + GitHub: <https://github.com/kaist-cp>
- Development machines: <https://dev.fearless.systems>
  + The `/home/$USER/local-home` directory is local/single SSD (not remote/replicated HDD like other directories in home).
    *WARNING*: this directory has a higher risk of data loss, e.g., due to media failure.
  + The `/home/$USER/share` directory is shared with lab members at `/home/_share/$USER`.
  + The `/home/$USER/share/www` directory is publicly accessible at <https://public.fearless.systems/$USER>.
    *WARNING*: it is open to the internet.
- VPNs
  + Server room: <https://rack.fearless.systems>
  + Office: <https://office.fearless.systems>
- Internal document: <https://git.fearless.systems/kaist-cp/infra-internal>
- Courses
  + Development machines: <https://cloud.fearless.systems>
  + CS431: <https://github.com/kaist-cp/cs431>
  + CS420: <https://github.com/kaist-cp/cs420>
  + CS220: <https://github.com/kaist-cp/cs220>

## Onboarding

- Email Jeehoon (`jeehoon.kang@kaist.ac.kr`) from your `{firstname}.{lastname}@kaist.ac.kr` account.

- Account (Google Workspace): Receive your `{firstname}.{lastname}@cp.kaist.ac.kr` Google Workspace account from Jeehoon.
  Use this account for all web services (except GitHub).

- [Calendar (Google)](https://calendar.google.com):
  Manage your schedule here.
  To arrange a meeting, simply create an event, include an agenda, and directly invite participants.

- [Email (Google)](https://mail.google.com)
    + Write [proper formal emails](https://www.wikihow.com/Write-a-Formal-Email). Avoid excessive email markup.
    + Check both `{firstname}.{lastname}@kaist.ac.kr` and `{firstname}.{lastname}@cp.kaist.ac.kr` email accounts.
      Jeehoon forwards emails from the former to the latter and checks them in Gmail.

- [Drive, Docs, Spreadsheet, Slide, Form (Google)](https://drive.google.com):
  Store all project-related files in the shared Google Drive.

- [Drive (Seafile)](https://drive.fearless.systems)

- [Chat (Zulip)](https://chat.fearless.systems)
    + Say hi in [this topic](https://chat.fearless.systems/#narrow/stream/112-general/topic/.EC.86.8C.EA.B0.9C) as soon as possible.
    + Zulip is our primary communication method.
    + To start a video call, click the Video button while writing a message, which creates a [Jitsi Meet](https://jitsi.fearless.systems) link.

- Git repositories
    + [GitLab](https://git.fearless.systems): Explore projects to find your interests.
    + GitHub: Join the [`kaist-cp` organization](https://github.com/kaist-cp). Display your real name in your public profile (Settings > Profile > Name). We prefer GitLab over GitHub.
    + For creating new organizations or repositories, ask Jeehoon.
    + Set up email notifications for mentions and issue/PR/MR comments.

- [Website]({{ site.baseurl }})
    + Create your website by sending a PR to [the website repository](https://github.com/kaist-cp/kaist-cp.github.io).
    + Regularly update your website.

- Development
    + Learn VSCode. 
      If you prefer editors like Vim or Emacs, it's acceptable, but remember VSCode is widely used.
    + Master Git with tutorials from [Atlassian](https://www.atlassian.com/git/tutorials) and [GitHub](https://lab.github.com/).
    + Understand SSH.
        * Generate an ed25519 SSH key: <https://www.ssh.com/academy/ssh/keygen>.
        * Authorize your key on servers: <https://www.ssh.com/academy/ssh/copy-id>. Avoid using passwords.
        * Set up your local SSH config: <https://linuxize.com/post/using-the-ssh-config-file>
        * Utilize `ssh-agent`.
    + Complete [The Missing Semester of Your CS Education](https://missing.csail.mit.edu/) ([Korean translation](https://missing-semester-kr.github.io/)), excluding "Editors (Vim)".
    + Use the development machines as [described here](#services).
