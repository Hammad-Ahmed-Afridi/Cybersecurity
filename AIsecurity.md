# Try Haack Me
## AI Security
- the first module focuses on foundational knowledge required for artificial intelligence like llms machine learning deep learning neural networks types of machine
  learning like supervised unsupervised semi supervised and reinforcement learning datasets ml algorithms nodes fine tuning black box white box models foundational
  models pre trained models model bias all of these concepts are mentioned in my ai repo in easy used terminologies
- as ai adooption is increasing day by day its becomes just like other system in an infra that is security is required ai security is the practice of securing ai tools
  models against adversaries attacks include prompt injection in which the attacker enters a well curated prompt which makes the ai go against its predefined rules for
  its behaviour which are also called guardrails and system prompts and make the ai model do wrong doings then we have data poisoning as we know that ai is trained on
  vast sets of data and that data if not properly cleaned and monitored and analyzed can cause the model to go against its desired state the data can be poisoned by an
  attacker and that data when taken is used for training ai models and if the neural network gets trained on it the output will be in accordance to the poisoned data then
  we have model theft that is the model properties are stolen as a whole or through its usage that is the model is prompted and the outputs are used to train an other
  model this is called distillation attack in which one model gets trained on another model structured outputs without requiring extensive gpus and data sets which
  reduces the cost of training the model and get good also than we have private information disclosure in which if the model is trained on data that included the private
  info outputs produces may contain that information 
- as ai is being adopted very fastly attackers are using it to their benefits like creating highly complex and dangerous malwares in matter of some time and using it
  against systems and also doing social engineering by creating highly accurate phishing emails cloning voices and creating deepfakes but as the attackers are using them
  security analyst and security engineers are also using them for their own benefits like using ml models to identify phishing emails with maximum positives by training
  them on large data sets of phishing emails and normal ones and then deploying them on security systems like siem and security engineers use them for having a teammate
  that tell them to perform certain actions that they may miss if they ddo it themselves on the systems for maximum security 
- we can secure ai models by properly configuring them using proper cleaned datasets implementing strict guardrails and system prompts and implementing rbac and
  strict access control and monitoring the deployed models and checking for anomalies and unusual behavior 
- prompting ai is giving it some text from user side so that it can analyze it and give answers the more detailed the prompt the more detailed and accurate the answer
  it is like garbage in garbage out this also goes for data also that the model is being trained on we have system prompt and user prompt user prompt is the text or
  prompt given by user system prompt are guidelines rules that are bolted in for the ai model to perform in a certain way that prompt is not visible to the end user
  we can giev ai prompts in a specific way for desired outcomes like first we give the context than the instructions that the output format and then certain rules to
  follow 
- ai models are being used in cybersecurity in a number of ways in digital forensics we have large sets of data and a human would take much time so the ai model is
  fed the dataset and it analyzes it correlates them and give output that is highly accurate if the prompts and detailed and the data is extensive same goes with great
  numeber of logs that are generated and ai models help in triaging alerst and correlating them also ml models can be used for detecting anomalies by first making them
  learn the normal state and then use it for abnormalities but as ai is very useful ai is also very probabilistic rather than deterministic that is same input can create
  completely different output and also i high number if false positives can be generated when relying solely on ml models also ai models are not transparent that is
  no one knows how and why ai made such an output and decision and can be sometimes biased so the oiutcomes can not be used in legal rulings where chain of custody is
  a must and also where findings are transparent that tells who found them ad why 
- ai is a system as a whole containing multiple ayers and just like any other system it also has vulnerabilities and needs security owasp top 10 for llm has the ten
  most common vulnerabilities and mitre atlas adverserial threat landscape for ai systems shows how these llm vulnerabilities are exploited by attacker and nist
  ai risk managemnt framework tells us how to protect them we also have a field called mlsecops which is the security of ml models or ai models from the start
- ai models is not a one surface application but the whole architecture is built upon number of tools like the models itself the user end app the the data the model is
  trained on the rag pipeline the vector database the system prompts so for this we can not implement one stop solution we have to implement multiple layer security
  we have a number of llm and ai model attacks and owasp top 10 for llm are propmt injection access privilages data posining model theft accessive trust supply chain
  system prompt leakage and many more we can use mitre atlas framework to study how llm attacks are carried out and use nist ai framework to put safeguards we can also
  implement system prompt hardening input validation data protection for supply chain least privilages and many more 
- prompt injection is done by manipulating the model and making it go against the guardrails it has and also leak the system prompt or make it do the work that it is
  not intended to do but this only works for that session then we have jailbraking that is making the model permanently go against its guardrails and rules and this
  can be done by a numebr of methods including prompt injection 
- we either use ai through apis and apps or self deploy it when using the apis we can only check for the things that are in front of us the cat interface the model
- behaviour and we can use the apis of well known providers for safety but still it is all balckbox that is we do not how it works how was it trained and on which data
  set and what tools it use and then we have deployed models on our own systems which we fine tune for specific purpose for safety we use model cards that has all the
  details about the model like the provider the data set on which it was trained and the pickle and safe tensor serialisation which tells us will the code be executed
  or not but best is safe tensor we can also do model scan using tools and once the model that is downloaded goes through all these methodologies it is safe to be
  used and deployed but still it should not be given access privilages 
- retrieval augmented generation rag is used to make llm use retrieval system for custom documents the documents are stored as embeddings that are basically vectors
  stored in vector database and when the ai system is prompted the prompt is taken and then the system prompt is included and then the system retrives the text that
  best matches to the prompt like closely related and then they are sent as one to the llm for generating a response in this system llm can not distinguish between
  the user prompt the system propmt and the retrived document so it if attacker manipulates the system to give off baad document like in rag system by injecteing it
  or abusing semantic relevance or do prompt injection or hijack system propmt in this way they can manipulate the model and make it give bad outputs for mitigating
  this the system prompts are hardened and the rag database should be secured and the user propmts should be distinguished by labelling or tagging and also monitoring
  the llm outputs and the rag database 
