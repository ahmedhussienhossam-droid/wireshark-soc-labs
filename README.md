# Wireshark SOC Labs – Networkwalks Internship

**Author:** Ahmed Hussien Said Hossam Eldin
**Program:** Cybersecurity Internship – Networkwalks Academy

This repo holds my results for the Wireshark SOC Labs I completed during the internship. Each lab gives a packet capture (PCAP) and a set of questions about what happened on the network. I answered them by analysing the capture in Wireshark.

## Results

| Lab | Topic | Date | Score |
|---|---|---|---|
| Lab 3 | Identify the attacker's IP | 30 Oct 2026 | 100 / 100 |
| Lab 4 | Follow TCP Stream | 30 Oct 2026 | 100 / 100 |
| Lab 5 | Follow TCP Stream, part 2 | 2 Nov 2026 | 90 / 100 |
| Lab 6 | HTTP plain text credentials | 3 Nov 2026 | 100 / 100 |
| Lab 7 | Brute force catch | 3 Nov 2026 | 100 / 100 |
| Lab 8 | VoIP call replay | 3 Nov 2026 | 100 / 100 |

The result card for each lab is in the [`results`](results) folder.

## What each lab covered

**Lab 3 – Identify the attacker's IP**
Filtering a capture for SYN packets to find who was scanning whom, then telling open ports from closed ones by looking at how the target replied. The traffic pattern was a port scan.

**Lab 4 – Follow TCP Stream**
Finding a chat session in the capture, locating its port and stream number, and using Follow TCP Stream to read the conversation.

**Lab 5 – Follow TCP Stream, part 2**
Going through HTTP traffic to find pages, a hidden stream, a file download and the status codes involved. This was the one where I lost marks, on the "code word" question.

**Lab 6 – HTTP plain text credentials**
Spotting a login done over plain HTTP, finding the POST request and reading the username and password straight from the packet details. It shows why unencrypted login pages are a problem.

**Lab 7 – Brute force catch**
Identifying repeated failed logins from one source against one target, then finding the point where an attempt succeeded.

**Lab 8 – VoIP call replay**
Looking at the call setup traffic and the voice stream in a capture: who called, who answered, and which codec was used.

## Tools

- Wireshark
- Networkwalks lab environment (see my [lab setup repo](https://github.com/ahmedhussienhossam-droid/networkwalks-lab-setup))

## Note

I haven't included the exact answers or flags for the labs, since they are graded exercises and other students are working through them too.
