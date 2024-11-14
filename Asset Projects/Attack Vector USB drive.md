# Scenario
You are part of the security team at Rhetorical Hospital and arrive to work one morning. On the ground of the parking lot, you find a USB stick with the hospital's logo printed on it. There’s no one else around who might have dropped it, so you decide to pick it up out of curiosity.

You bring the USB drive back to your office where the team has virtualization software installed on a workstation. Virtualization software can be used for this very purpose because it’s one of the only ways to safely investigate an unfamiliar USB stick. The  software works by running a simulated instance of the computer on the same workstation. This simulation isn’t connected to other files or networks, so the USB drive can’t affect other systems if it happens to be infected with malicious software.

## Exercise
- These are the contents of the USB:
![Attack_Vector_USB](https://github.com/Cr1msonPho3nix/Asset_Management/blob/main/img/Attack%20Vector%20USB/1.1.Attack_Vector_USB.png)<br>

| Subject | Description |
|--       |--           |
| Contents | - Some family photos can be found on a folder.<br>- Shift Schedules and Employee budget files.<br>- Personal stuff shoudln't be put together with job files. |
| Attacker Mindset | - Family photos can be used to blackmail Jorge into more shaddy practices, like use him as an insider.<br>- Shift Schedules and Employee budget are files that can grant some information about some aspects of the business.<br>- The wedding and vacation ideas files grants information on when Jorge won't be working, so an attacker can use that to prepare some kind of attack on his name in that period of time. |
| Risk Analysis | - A hidden plug-in software can be installed on the driver, so if an oblivious employee finds it and plugs it in their computer it can infect that terminal and even expand into the internal network.<br>- Some files on the drive contain sensitive information, like family photos and economical information, from Jorge and the organization, which can be used against them.<br>- Jorge can easily be blackmailed with his family photos to do simple but really dangerous tasks, such as plug-in provided drivers in high privilege terminals or send phishing e-mails to high privilege team mates. |