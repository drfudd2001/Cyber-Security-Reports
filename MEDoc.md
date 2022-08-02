# Malware infecting Ukrainian tax-filing software

- What type of attack was this?

This is a worm, or self-spreading malware attack. It is believed to have spread originally via email, but quickly attached itself to self-updating software developed by an accounting firm in Ukraine, MEDoc. The source of the assault is still unknown, however the company MEDoc now denies responsibility for the creation or intentional propagation of this malware. Ukraine accounted for around 80% of all infections, with Germany accounting for the remaining 9%.

- How was the vulnerability discovered and the attackers exploit this?

This worm exploits a number of vulnerabilities. This worm appears to attach to and infect the companies' automatic software updating tools used in their accounting software. Once infected, the computer will seek to spread to other computers on the same network. This is accomplished by an SMB or Server Message Block exploit known as EternalBlue. Once infected, it will attempt to hijack administrator tools with elevated user access in order to remotely manipulate the victim's PC and install malware. Finally, the Master File Table of the infected computer is assaulted in order to confuse the location indexes of files on the PC. After a short period of time, the computer will reboot and issue the following ultimatum to the user: Provide a payment to unlock and access your information.

- Were there security measures that could have been taken in order to prevent this attack?

Unlike traditional worms, which need consumers to accidentally click on a link in an email or message, this attack is carried out using software update tools from multiple organizations. If they aren't already, the update tool might apply SHA or MD5 verification methods before downloading and installing new updates. If this was employed and the attackers also evaded it, more tight testing on update verification and access to update pushes could have been beneficial. Overall, attackers will crack these and find a way in. A two-step verification process requiring several users to review and modify production updates before they can be posted may have been the best option.
