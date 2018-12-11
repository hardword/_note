#####GDPR Penalty#####

Two tiers of administrative fines

* Up to €10 million, or 2% annual global turnover – whichever is higher
* Up to €20 million, or 4% annual global turnover – whichever is higher

#####The STRIDE Threat Model#####

* **S** (*Spoofing*) : Using another/legit user’s authentication information 
* **T** (*Tampering*) : Unauthorized changes made to persistent data (stored/in-transport) 
* **R** (*Repudiation*) : Ability to trace user activities to provide evidence
* **I** (*Information Disclosure*) : The exposure of information to the unauthorized (stored/in-transport) 
* **D** (*Denial of Service*) : The server or service is made temporarily unavailable
* **E** (*Elevation of Privilege*) : The unprivileged find a way to gain authorization to compromise the system.

#####The DREAD risk assessment model#####

* **DREAD** (*Damage, Reproducibility, Exploitability, Affected Users, and Discoverability*)  
	* A scale from 0-10 is usually used in all categories, save for discoverability which is commonly set to 10 on the grounds that any threat will eventually be discovered.
	* *There has been a fair amount of discussion concerning Discoverability, and whether encouraging security professionals to minimize discoverability would in turn favor the deprecated approach of security through obscurity.*

#####Fuzzers to Try#####
* [radamsa](https://gitlab.com/akihe/radamsa)
* [AFL](http://lcamtuf.coredump.cx/afl/) - American Fuzzy Lop
* [oss-fuzz](https://github.com/google/oss-fuzz) - Google

#####Debugging Tools to Try#####
* gdb
* [valgrind](http://www.valgrind.org/)
* strace
* ltrace

#####Defining Requirements#####
a.k.a "user stories" (Security: "evil user stories")
Good user stories are something that one can INVEST into, and they can be used to create SMART tasks.

* INVEST:
	* Independent
	* Negotiable
	* Valuable
	* Estimable
	* Small
	* Testable

* SMART:
	* Specific
	* Measurable
	* Achievable
	* Relevant
	* Time-boxed

OWASP [Proactive Controls](https://www.owasp.org/index.php/OWASP_Proactive_Controls)

#####DevOps#####
* small, continuous and iterative changes
* minimizing unnecessary delays
* maximizing efficiency 
* need for the automatization, optimization, and simplification
* transparency and auditability (agile - transparent to the customers)

* **Canary** releases: 
	1. Changes can be pushed only to a small percentage of the nodes to be updated. 
	2. Observation of the nodes that have the newer code in place, and see if the work as intended. 
	3. The changes can be deployed to the rest of the network if everything is okay.
