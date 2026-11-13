# Cybersecurity: Network Threats & Attack Memory Tricks

**ITAI 4370 — Module 8 | Study notes**

These notes use technical definitions, examples, movie/story analogies, memory tricks, and accuracy distinctions. **The film and story references are analogies, not documented examples of cyberattacks.**

## 1. Eavesdropping (passive interception)
- **Definition:** Secretly monitoring communications without changing them.
- **Example:** A sniffer captures unencrypted traffic or a wiretap records a conversation.
- **Analogy:** *Goodfellas* — surveillance of Henry Hill and associates.
- **Memory trick:** Someone is listening without joining the conversation.
- **Accuracy note:** Not limited to telephone taps; encryption can protect message contents.

## 2. Man-in-the-Middle (MITM)
- **Definition:** An attacker places themselves in a communication path to intercept, relay, or alter traffic.
- **Example:** A malicious Wi-Fi hotspot relays traffic while attempting interception.
- **Analogy:** *The Departed* — Billy Costigan passes information between groups.
- **Memory trick:** A hidden middleman accesses what passes between parties.
- **Accuracy note:** A human mole is an analogy, not literally a network MITM attack.

## 3. DoS vs. DDoS
- **Definition:** Denial-of-Service disrupts availability; Distributed Denial-of-Service uses multiple attacking sources.
- **Example:** Requests exhaust service capacity and block legitimate users.
- **Analogy:** A restaurant entrance overwhelmed by people.
- **Memory trick:** DoS = one source; DDoS = many sources.
- **Accuracy note:** DoS can exploit implementation weaknesses without huge traffic volumes.

## 4. Targeted exploit (“ninja strike”)
- **Definition:** A deliberately crafted input or packet exploits a specific system weakness.
- **Example:** A malformed request causes a vulnerable implementation to crash or behave unexpectedly.
- **Analogy:** Samson attacks a temple's supporting pillars; *Captain Phillips* evokes takeover.
- **Memory trick:** A precise strike at a weakness rather than sheer volume.
- **Accuracy note:** “Ninja attack” is not a standardized attack name; takeover is not guaranteed.

## 5. SYN flood (“death by a thousand cuts”)
- **Definition:** A DoS attack exploiting TCP connection setup through many half-open connections.
- **Example:** SYN → SYN-ACK → ACK is the normal handshake; in a flood, many final ACKs never arrive.
- **Analogy:** *Jackass / Bad Grandpa* — repeated knocking without completing the conversation.
- **Memory trick:** Unanswered knocks keep legitimate visitors waiting.
- **Accuracy note:** SYN floods became prominent in 1996; “death by a thousand cuts” is a nickname.

## 6. Rogue base station
- **Definition:** An unauthorized station impersonates cellular infrastructure to interact with nearby devices.
- **Example:** Depending on network security, it may collect identifiers, interfere with service, or support tracking.
- **Analogy:** *Superbad* — McLovin's fake ID.
- **Memory trick:** Fake ID = fake identity = fake cell tower.
- **Accuracy note:** McLovin did not impersonate police; fake towers cannot automatically decrypt all calls or messages.

## 7. Protocol exploits
- **Definition:** Attacks abusing network protocol design or implementation weaknesses.
- **Example:** ARP spoofing, DNS spoofing, or TCP session hijacking.
- **Analogy:** *Pirates of the Caribbean* — Jack Sparrow uses loopholes in the Pirate Code.
- **Memory trick:** Protocol = communication rules; exploit = abuse a weakness.
- **Accuracy note:** Fictional loopholes are analogies; real attacks require technical weaknesses.

## 8. Firmware attacks
- **Definition:** Compromise of low-level software running on hardware devices.
- **Example:** Malicious router or computer firmware changes behavior, persists, or enables privileged access.
- **Analogy:** *Iron Man* — Obadiah Stane's hidden sabotage.
- **Memory trick:** The danger is hidden inside the device.
- **Accuracy note:** Firmware is not hardware; persistence after OS reinstall is possible, not guaranteed.

## 9. Supply chain attacks
- **Definition:** Compromise of a trusted vendor, dependency, update, component, or delivery path before reaching a victim.
- **Example:** The 2020 SolarWinds compromise distributed malicious code through software updates.
- **Analogy:** The Trojan Horse.
- **Memory trick:** The attack is already inside the package before it arrives.
- **Accuracy note:** Supply chain compromises can affect hardware, software, or firmware.

## Quick comparison

| Threat | Core idea | Memory aid |
|---|---|---|
| Eavesdropping | Listen secretly | Goodfellas |
| MITM | Intercept communication path | The Departed |
| DoS / DDoS | Disrupt availability | Crowded restaurant |
| Targeted exploit | Exploit specific weakness | Samson |
| SYN flood | Incomplete TCP handshakes | Jackass knocking |
| Rogue base station | Fake cellular tower | McLovin fake ID |
| Protocol exploit | Abuse network rules | Jack Sparrow |
| Firmware attack | Compromise embedded software | Iron Man hidden sabotage |
| Supply chain attack | Compromise trusted delivery | Trojan Horse |

*Adapted from the supplied “Cybersecurity: Network Threats & Attack Memory Tricks” study notes document.*
