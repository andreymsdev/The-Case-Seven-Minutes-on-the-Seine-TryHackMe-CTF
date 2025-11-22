# The Case: Seven Minutes on the Seine — TryHackMe CTF

Well, here we go again.  

You are the analyst on call after a hi-vis crew struck the **Galerie d’Apollon** and fled toward the river. Investigate using only open sources.  

**Tips:** Google Maps and browser inspection tools.  

---

## The Incident

Something audacious unfolded beneath the glass pyramid.  

In the early hours, a crew in hi-vis vests breached the Galerie d’Apollon inside the Louvre. Security feeds went dark, and seven minutes later, the team disappeared toward the river.  

You are the first analyst on call. Your mission is to reconstruct the details of the heist using open-source intelligence and online reports. The museum is under pressure, international alerts are spreading, and the press is already digging for answers.  

Gather and verify information from public sources: museum pages, heritage archives, news coverage, social media, and open databases.  

---

## Technical Setup

Click the *Start Machine* button and access the portal via the link provided.  
Note that the machine may take 2–3 minutes to initialise.  

However, the machine didn’t work for me, so I just typed the target IP directly into the browser.  

At first, I tried using AI, but it wasn’t as easy as it looked — every answer came out wrong.  
So I had to go back to the old-school method: searching manually through the Louvre website and Google Maps.  

Fortunately, the questions themselves contained a lot of hints. I started a deep search on Google Maps.  

---

## First Question

Here’s the first question (the rest follows the same logic, searching the web for clues):  

**`PORTE_DES_LIONS-22_OCT_2024`**

---

## Louvre Protocol

A recent news report referencing an earlier audit of the museum’s surveillance network revealed serious weaknesses:  

- Outdated servers  
- Inconsistent camera coverage  
- Weak password policy  

As the on-call CCTV analyst, your job is to verify whether the credential clues in those reports are valid against the system and then use them to review the footage from the day of the incident, documenting every step and source.  

You may refer to online sources to identify the correct credential pair for this lab environment and review the footage from the day of the incident.  

Click the *Start Machine* button and access the portal via the link provided.  
Note that the machine may take 2–3 minutes to initialise.  

This part was the easiest one: I simply looked up the leaked Louvre password (it was very obvious), logged in, and then searched for the specific date on the security cameras.  

---

## Personal Comment

The importance of the *“Seven Minutes on the Seine”* CTF lies in how it teaches practical OSINT and cybersecurity investigation skills through a realistic, story-driven scenario. It shows how open-source intelligence can be leveraged to reconstruct events, trace movements, and uncover vulnerabilities in critical systems.  

What struck me most is the sheer impact of something as simple as a password.  
A single weak credential can compromise an entire network, disable surveillance, and open the door to a full-scale breach.  
