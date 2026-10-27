# a)	SCIENCE HUNT

I started with following the instructions Start Your Research with a Review Article guide. 
I searched google scholar for “software vulnerability detection”. It returned many articles, then I searched again with “software vulnerability detection review”. After going through few links, I chose “Real-time privacy vulnerability detection techniques in software development: A Systematic Literature Review”. I checked for its JUFO rating and the journal was listed as Level 2.

# b)	REVIEW THE REVIEW

## What are the key areas being researched?
- Methods for finding privacy problems: The article explores different ways to identify privacy vulnerabilities in software, including static analysis, dynamic analysis and machine-learning-based methods.
- Security tools: It examines tools that can help developers detect privacy issues in their coding environments, mobile applications and network systems.
- Integration into software development: Another focus is how privacy checks can be included in everyday development activities and automated testing pipelines.
- Privacy from the beginning: The review considers how privacy protection can be built into software during the design and development stages instead of being added later.
- Limitations of existing solutions: The authors investigate problems such as detection accuracy, processing speed, scalability and the practical usability of security tools.

## What's widely agreed upon?
- Finding problems early is beneficial: Detecting privacy issues before software is released can make them easier to address and reduce the risk of exposing sensitive information.
- Different methods serve different purposes: Each detection technique has its own advantages and weaknesses. Combining approaches may help identify a wider range of problems.
- Tools should support developers: Security checks should fit into normal development work without causing unnecessary delays or making the process complicated.
- Incorrect warnings are a problem: When tools report issues that are not genuine vulnerabilities, developers must spend additional time investigating them.
- Privacy needs continuous attention: Privacy protection should be considered throughout software development, rather than only during the final testing stage.

## What are the open questions?
- Improving performance: How can privacy detection tools handle large software projects while providing results quickly?
- Reducing incorrect warnings: How can developers identify more genuine vulnerabilities while avoiding unnecessary alerts?
- Making tools easier to use: How can security tools present their findings clearly so developers can understand and fix problems more easily?
- Supporting different environments: How can privacy detection work consistently across different programming languages, development tools and CI/CD pipelines?
- Measuring effectiveness: What evaluation methods can reliably show which detection techniques work best in real-world software projects?
- Using newer technologies: Can machine learning and other emerging techniques improve the accuracy and speed of privacy vulnerability detection without introducing additional limitations?


# C) THREAT MODELING QUICKRUN
## 1. Company
Company: A fictional IT consultancy that develops software applications and provides cloud-based solutions to business customers.
Crown jewels
The company's most important assets are:
- Confidential information: Customer records, business data, application source code and login credentials.
- Business operations: The systems and services required to deliver projects and support customers.
- Reputation: The trust built with customers and business partners.
- Financial resources: Company income, customer contracts and money needed to recover from security incidents.

## 2. Bad guys
Cybercriminals may target the company to steal valuable information, demand ransom or make money by selling compromised data.
According to the COI model:
- Capability: Attackers may have the skills and tools to send convincing phishing emails, steal passwords or exploit weaknesses in online applications.
- Opportunity: Employees access cloud platforms and company systems over the internet, creating potential entry points for attackers.
- Intent: Their objective may be to obtain money through extortion, sell confidential information or disrupt the company's services.

## 3. Identify and estimate two risks
The following figures are hypothetical estimates of the financial loss that could result from each incident.  

Risk 1: A cybercriminal gains access to a cloud account and exposes confidential customer information.  

Annual likelihood 20%  
Estimated loss per incident €100,000  
Expected annual loss €20,000

Risk 2: A ransomware attack blocks access to business systems, interrupting projects and customer services.  

Annual likelihood 10%  
Estimated loss per incident €60,000  
Expected annual loss €6,000

The expected annual loss is calculated by multiplying the probability of an incident by its estimated financial impact.
- Risk 1: 0.20 × €100,000 = €20,000
- Risk 2: 0.10 × €60 = €6,000
  
Biggest risk is Risk 1 because it is estimated as €20,000

## 4. What should we do about the biggest risk? (META)
Decision: Mitigate.

The company should reduce the likelihood and impact of stolen cloud credentials by:
- Enforcing multifactor authentication (MFA) on all cloud accounts.
- Restricting access to sensitive data based on employees' roles.
- Storing passwords and application secrets securely.
- Monitoring suspicious login attempts and reviewing account permissions regularly.

Expected result: Assume these measures reduce the likelihood of a breach from 20% to 5% per year and the potential impact from €100,000 to €60,000.

Revised estimated annual loss:
5% × €60,000 = €3,000

This reduces the estimated annual loss from €20,000 to €3,000, an 85% reduction.

The figures are hypothetical targets. Actual risk reduction would need to be evaluated after the security measures are implemented.

