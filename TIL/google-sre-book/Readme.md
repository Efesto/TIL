## SRE Book from Google
https://landing.google.com/sre/sre-book/toc/

> Hope is not a strategy

- The classic Developers + Operators approach to build and maintain systems is surpassed
  - It generates contrast between desire for a fast system change delivery vs desire for system stability
- SRE can be seen as a subset of Devops
- An SRE team is composed by a variagated set of skills spacing from developing to system maintenance
  - People who gets easily irritated by repeatitive and boring manual tasks and therefor wish to automate them are a good fit
  - *Toil* is the word
- SRE embraces errors as a natural component of a system
  - Defines *Errors budget* as the possible slack to conceed to a system in terms of errors
  - A new feature takes a certain amount of error budget and any new increment in complexity of the system requires a payment of it
  - 70% of outages are due changes to a live system
  
# Emergency Response
- A playbook listing what to do in an emergency situation used by even an unexperienced operator is more effective than an expert without it


# Capacity Planning
- Capacity planning should take in consideration organic and inorganic growth in product usage
  - Organic - product adoption and usage
  - Inorganic - events like launches, marketing campaigns and so on
- Several steps for capacity planning are mandatory:
  - Organic demand forecast
  - Knowledge of inorganic demand
  - Regular load testing

# SRE Principles
- Embracing Risk
- Eliminating Toil
- SLOs instead of SLAs
- Monitoring
- Simplicity

- Time based availability `Availability = uptime / (uptime + downtime)`
- Aggregate availability `successful requests / total requests`
  - Useful for systems that do not typically serve end users directly

(Continues from CHP 3)
