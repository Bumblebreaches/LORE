# Learnings on Options & Reasons for Exploitation

## What is L.O.R.E

This is a work-in-progress reference tool of common scaled abuse actor goals, incentives, methods, and inversely platform surfaces, policies, interventions, and design considerations. Similar to Security's [MITRE ATT&CK](https://attack.mitre.org/) framework, the much older [Threat Hunting Project](https://github.com/ThreatHuntingProject/ThreatHunting/issues) or the [Malpedia](https://malpedia.caad.fkie.fraunhofer.de/) for focused on online platform safety scaled abuses instead such as toll fraud, infrastructure abuse, spam, harassment, account generation, and scraping.

This is organized as a series of definitions and matrixes and is intended to be used by online platforms at any stage to perform risk assessments and share options and and source new means of mitigating scaled abuse in accompaniment with their typical operating processes. 


--- 

## Contributing to LORE

This is very much so a proposal and work in progress that will be updated regularly. Please feel free to take this initial start and create versions that suit your needs or if you'd like to collaborate on normalizing and populating this please reach out to me to see about helping with admin, or suggest changes as you see fit. 

I am working on this not as a representative of my workplace so responses may be delayed.

Long term after additional population and normalizaiton of terms this repository will move to also be searchable via tags and available in formats to ease requesting programatically.

---

## Standard Components

### User Journey
> This is associated with a single Abuse Category and Goal, and an aggregation of Abuse Objective, Platform Feature, Abuse Incentives (unique column to the journey), Abuse Method, and Platform Mitigations along with associated examples. 

### Abuse Category
> This is the meta category that a goal fixates toward. This is a limited category and contains broad desires based on the type of harm only. Examples include Profit, Hate & Harassment, Theft, Disruption, etc. There will be one of these per User Journey.

### Abuse Goals 
> This is a more concrete example of what an actor really wants from the platform from a type of abuse. A singular goal is present for a User Journey but has multiple objectives due to many different incentives and may touch many features. Failed goals and therefore failed User Journeys may overlap with other Journeys at the intersection of where it failed or succeeded. An example would be a goal of "Selling Fully Verified Accounts" may begin a User Journey to a spam actor who purchases the account whose goal is "Mass Comment Links". 

### Abuse Methods
> Similar to category this is surprisingly going to be kept very broad. There are countless means of spoofing, botting, and exploiting but this is going to focus on the broad strokes of what the actor is using to **achieve scale**, not necessarily to avoid detection which may be the way in which they adjust the configuration of their method but still utilize the same means of scaling. Examples include automation through headless scripting, automation via browser emulation, or mass mobilization of human users via a variety of intentions.

### Abuse Objectives
> A single user journey will have many Abuse Objectives and each Objective will help describe what the spammer or abuse actor wants from each event they typically perform. This should generally be quite specific and typically will relate closely to the feature it is involved with, but could be more broad for example in instances where an actor may be expected to adjust it or if its specifically not tied with any feature or involves off platform behavior. 


### Platform Features
> These are the broad surfaces and features that many platforms will have in common that is at risk of abuse. Internally this could correlate to a single API endpoint, or a whole workflow, or a single feature, however you define that (as I know we all do differently). Examples include account creation, payments, free trials, verification, messaging, interventions, uploads, calling, and the like. As time goes on it may be viable to split into various categories but until and when there is enough terms to necessitate that we'll take a stab at this.

### Platform Mitigations
> These are either subtyped as **Interventions** or **Designs**. Interventions are intended to validate activity with the intent to disrupt or stop scaling reactively while Designs are intended to alter the relationship between the platform and the actors by changing a Feature/Surface to alter an incentive. Each mitigation will have its own details, contexts, and resources. 

### Examples
> This is any place to upload research, RFCs, Specs, post-mortems, breakdowns, recommendations, implementationg guides, tools or the like to be later tagged and associated with either Mitigations (Design or Intervention) or a User Journey or Goal. 

---

## BYOB Components

### Abuse Troupe:
> We have enough names and codewords in Security for threat actor groups so we don't need those here necessarily other than for example purposes unless the need arises. Due to widespread tool sharing and tool development Troupe here does not mean a singular threat actor organization but instead a "whichever useful" determination of a collection of related User Journeys. A User Journey does not have to have a Troupe, but can if its associated with other Journeys. 

### Platform Policies
> These will be unique to your organization. If you use the information in LORE to conduct risk assessments you'll likely want to ascribe a given goal to what platform policy/law/requirement it is likely to violate. For example, Bulk Creating/Selling Accounts may violate your Terms of Use. 

### Platform Data
> This is for any metrics, supporting documentation on features, queries, code, signal, available interventions or other information that is relevant to you if you are using this in the form of a risk assessment or product design.

---
