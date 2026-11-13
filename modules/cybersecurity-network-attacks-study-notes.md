# Cybersecurity: Network Threats & Attack Memory Tricks

Cleaned study notes | Definitions, technical examples, movie references, and important distinctions

## 1. Eavesdropping (passive interception)
**Definition:** Secretly monitoring communications without changing them.

**How it works / example:** A network sniffer captures unencrypted traffic, or a wiretap records a conversation.

**Movie or story analogy:** Goodfellas: law-enforcement surveillance of Henry Hill and associates is a reminder of secretly listening.

**Memory trick:** Someone is listening without joining the conversation.

**Accuracy note:** Not limited to physical telephone taps; encrypted traffic may prevent the attacker from reading message contents.

## 2. Man-in-the-Middle (MITM)
**Definition:** An attacker places themselves in the communication path and can intercept, relay, or alter traffic.

**How it works / example:** A malicious Wi-Fi hotspot may relay traffic between a user and a network while attempting interception.

**Movie or story analogy:** The Departed: Billy Costigan is a mole passing information between groups.

**Memory trick:** A hidden middleman has access to what passes between parties.

**Accuracy note:** A human mole is only an analogy, not literally a network MITM attack.

## 3. DoS vs. DDoS
**Definition:** Denial-of-Service disrupts availability; Distributed Denial-of-Service uses multiple attacking sources.

**How it works / example:** Many requests exhaust a service’s capacity, keeping legitimate users out.

**Movie or story analogy:** A restaurant entrance is overwhelmed by people so paying customers cannot enter.

**Memory trick:** DoS = one source; DDoS = many sources.

**Accuracy note:** A DoS attack need not use huge traffic; some exploit implementation weaknesses.

## 4. Targeted exploit (your “ninja strike”)
**Definition:** A deliberately crafted input or packet exploits a specific weakness in a system.

**How it works / example:** A malformed request triggers a vulnerable implementation; effects vary from crashes to unauthorized behavior.

**Movie or story analogy:** Samson brings down a temple by attacking its supporting pillars; Captain Phillips “I’m the captain now” recalls takeover.

**Memory trick:** A precise strike at a weakness rather than sheer volume.

**Accuracy note:** “Ninja attack” is a memory nickname, not a standardized technical attack name. A targeted exploit does not necessarily take over a system.

## 5. SYN flood (“death by a thousand cuts”)
**Definition:** A DoS attack that exploits TCP connection setup by creating many half-open connections.

**How it works / example:** Normal handshake: SYN → SYN-ACK → ACK. During a flood, many final ACKs do not arrive, consuming resources.

**Movie or story analogy:** Jackass / Bad Grandpa: someone keeps knocking at a door and never completes the conversation.

**Memory trick:** Repeated unanswered knocks prevent attention to legitimate visitors.

**Accuracy note:** SYN flooding became especially prominent in 1996. “Death by a thousand cuts” is a nickname, not the formal term.

## 6. Rogue base station
**Definition:** An unauthorized station impersonates cellular network infrastructure to interact with nearby devices.

**How it works / example:** Depending on network security, it can collect identifiers, interfere with service, or support tracking.

**Movie or story analogy:** Superbad: McLovin’s fake ID presents a false identity, just as a fake tower pretends to be legitimate.

**Memory trick:** McLovin’s fake ID = fake identity = fake cell tower.

**Accuracy note:** McLovin was not pretending to be a police officer. Fake towers cannot automatically decrypt all calls or messages.

## 7. Protocol exploits
**Definition:** Attacks that abuse weaknesses in network protocol design or implementation.

**How it works / example:** ARP spoofing sends misleading local address mappings; DNS spoofing provides false destination information; TCP session hijacking abuses a connection.

**Movie or story analogy:** Pirates of the Caribbean: Jack Sparrow bends the Pirate Code and uses loopholes.

**Memory trick:** Protocol = communication rules; exploit = take advantage of a weakness.

**Accuracy note:** A fictional rule loophole is an analogy. Real exploits depend on concrete technical weaknesses.

## 8. Firmware attacks
**Definition:** Attacks that compromise low-level software running on hardware devices.

**How it works / example:** Malicious firmware on a router or computer may change behavior, persist, or give an attacker privileged access.

**Movie or story analogy:** Iron Man: Obadiah Stane’s hidden sabotage from inside Stark Industries evokes a hidden compromise within a trusted machine.

**Memory trick:** The danger is hidden inside the device.

**Accuracy note:** Firmware is not identical to hardware, and persistence after an OS reinstall is possible but not guaranteed.

## 9. Supply chain attacks
**Definition:** Attacks that compromise a trusted vendor, component, dependency, update, or delivery pathway before it reaches the victim.

**How it works / example:** The 2020 SolarWinds compromise distributed malicious code through legitimate-looking software updates.

**Movie or story analogy:** Trojan Horse: danger enters hidden inside an apparently acceptable gift.

**Memory trick:** The attack is already in the package before it arrives.

**Accuracy note:** A supply chain compromise may target software or hardware; it can also deliver malicious firmware.

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

**Study note:** Film and story examples are analogies, not documented instances of the corresponding cyberattacks.
