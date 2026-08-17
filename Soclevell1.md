# Try Hack Me
## Soc Level 1
- in the world of cybersecurity the biggest risk are humans humans are hacked they are the weakest link in the cybersecurity and this happens by manipulation or taking
  advantage of emotions and othe rfactors and this whole is called social engineering number of ways are selected or used for exploiting humans like phishing
  vishing smishing and with the advancements of ai these attacks have became more commmon and more dangerous and made everyone capable of carrying out these attacks
  the attacks that specifically rose because of ai are deepfakes that are creating fake videos or voices that look hyper realistic and familiar
- systems include the machines that are being used in an organization or a place like computers laptops servers mobiles connected together to each other in lans and outside
  through wans and routers switched and firewalls are being used but if these systems are outdated that is using old softwares not patching them or upgrading them
  fixing their vulnerabilities then they  will be exploited by attackers if weak or default passwords are being used security configurations are not properly set then
  they will pose serious risk 
- in cyersecurity we can implement the most robust systems and make an outstanding security posture but if the humans as the weakest link are not trained they are not
  proper trianing than the security systems are of no use becasue an attacker can exploit the human emotions and get access to system and from then on it is easy for the
  adversary if skilled to gain foothold do lateral movement and privilage escalation and do serious level of destruction 
- in security operation centre soc we have teams and they consists of people like soc analysts security engineers soc engineers incident responders malware analysts
  ciso soc manager and many more we also have a number of tools being used in soc like siem security information and event management edr endpoint detection and response
  soar security orchestration automation and response 
- on every device a number of activities happen that are called events these events are logged in structured manner in a specific location these are used for analysis and
  monitoring these logs are being used by soc teams for providing security by monitoring actions on devices but as in an organization their are a number of devices it
  becomes difficult so these logs are forwarded to a central system called siem for a centralized analysis and itr becomes easy for monitoring edr is used for
  detecting activities on endpoints and taking actions against anomalies they also provide centralized lookups but the difference between an edr and siem is that siem is
  mostly used for entire network analysis and detections but edr is specifically used for endpoints that is devices that are connected to each other in a network
  and the other difference is that siem can not take actiosn it can only collect aggregate noramlize and correlate logs and display them in a structured format but edr
  can take actions from the centralized hub then we have soar which is used for automating repetitive tasks becasue in soc environments their are numerous events being
  collected from network and devices and managing every one of them becomes difficult so soar is used in which a serious of steps and actiosn are predefined and are taken
  if those are needed nowadays every tool is being centralized in a dashboard so that is becomes more easy for soc teams to manage everything
- alerts are the important components of a soc environment and they appear constantly and every second and must be dealt with and the dealing should be in such a way that
  the important ones are dealt with care and precautions and given full concentration and the normal ones should also be inspected but if it is a normal system activity
  the alert can be dropped this is called alert triaging that is prioritizing what is necessary and documneting investiigating and escalating and solving them we have
  alert severity ranging from low medium high and critical and the alerts that are old and also are critical should be dealt with first because attacker has
  already gained foothold and may have ampped the entire system as comapred to the new attacker and also proper documentation should be made before escalting to
  soc level 2
- in soc teams and soc environments we have terms that are being used that give us metrics on which we can identify the competency of the soc team and environment
  like mean time to detect mttd mean time to respond mttr and false positive percentage and true positive percentage
- soc teams have workbooks or playbooks or runbooks these books include guides and instructions to be followed when an incident happens and the steps include like protect
  detect respond and recover and post incident steps these are constantly updated and maintained and they are neccessary for soc teams as during attacks the envirnment
  becomes stressfull and without any guide it becomes difficult to mitigate the attack 
- pyramid of pain is a diagram or lets say a guide that needs to be known in order to make attacks less frequent and more costly and tine consuming for attackers
  first we have hash values as many tools out their like virus total that checks a file hash against known hashes that were malicious in a number of tools or app
  like app.any.run that lets us give browser based sandbox to test the malware but this can easily be tricked becasue as we know just changing a single character in a
  hash file can change the entire hash of that file so the attacker can tricj these tools and tehy can bypass rules or signatures so we can not only depend on hashes
  then we have ip addresses ip addresses that are malicious can be tested by the same two tools as well as ip checkers for locations but ips can be spoofed and they can
  be cosntantly changed by attackers thay can also use botnets in which the source ip that is cc server can become difficult to detect so we can not only rely on
  ips as well then wehave domaian same case domains can also be checked for previous maliciosu activities but attackers can but domains from trusted parties so this is
  also not effective that much then we have ttps that is tactics techniques and procedures if we have well erquipped systesm in place people trained and the ttps
  of the attackers are known so even if they use diffirent tools the core method philosophy will be the same so it becomes easier for defenders to catch attackers and
  the attackers are left with no choice but to spend more time effort and money for workarounds 
- cyber kill chain is a framework that tells us about the attack from beginning till the end from reconaissance stage to weaponization to delivery to exploitations to
  installation to command and control to exfiltration and this framework became old so a new framework came called unified kill chain and includes reconaissance stage
  to weaponization to delivery to exploitations to installation to lateral mocemnet to command and control to privilege escalation to data discovery to exfiltration
- mitre is a open knowledge base for attacker tactics techniques and procedures used we have a number of frameworks that are being given freely by mitre that are
  mitre attack mitre atlas mitre defend mitre attack which stands for attacker tactic techniques and common knowledge tells us why attacker performed certain
  actions which is tactic and then tells us how the actions were performed which is techniques and procedures mitre atlas stands for adversarial threat landscape for ai
  systems for attacks on ai systems and mitre defend stands for detection denial and disruption for security against these attacks 
- phishing is a social engineering attack that is used to exploit humans for delivering malware in to the systems or networks phishing is mostly done by emails in which
  well crafted emails are made impersonating legitimate users or organizations and sent to users so that they interact with it either by clicking a malicious link which
  will direct them to a specific website or either downloading a file which is executable which will execute code in the background nowadays as ai became more common
  phishing attacks got perfected that is attacker can craft well curated emails that are highly accurate and also personnel this happens because of ai speed of
  developement phishing can be detected in a number of ways like the use of malicios link generalized audience sense of urgency links to malicious websites .exe
  extension files attached and other as well we can use tools like virus total for detecting the links and file hashes against known malware database and we can use
  browser based sandboxes to interact with the files and links so that our original pc does not get infected even if we interact with it we can also use phishtool as well
