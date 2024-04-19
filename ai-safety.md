# AI Safety

## Intellectual Property

Regardless of your industry, generative AI tools like ChatGPT, Bard, and Bing can be useful in improving your work productivity. You can use generative AI tools for various tasks, from editing emails to producing boilerplate code in a new programming language. 

However, there are several Intellectual Property (IP) considerations to remember when using these tools in a work context. Let's start with one real-world example that will give you an idea of how problematic data privacy can be with Generative AI.

### **How AI Researchers Hacked GPT to Get NYT Staff Emails**

In October 2023, Indiana University researchers fine-tuned OpenAI’s GPT-3.5 API to extract emails for over 30 employees at the NYT. Although many of the personal email addresses for the Times employees had typos, about 80% of the work emails returned were completely correct. Most of these NYT work email addresses were publicly available through email. Still, this story rings alarms about the risk of open-source generative AI tools revealing sensitive information – despite safeguards put into place.

### How do Generative AI Tools Use Our Data

Tools like ChatGPT are trained on vast amounts of text, which may or may not contain personal information. This training data informs the tool but is not supposed to be recalled verbatim. However, the Indiana study that uncovered the NYT emails shows how the LLM’s memory can be jogged to retain precise personal information, with just a bit of fine-tuning.

By default, when you use ChatGPT, OpenAI will save data such as your conversation history, as well as account details like name, email, IP address, and device information. This collected data can be used to train and improve future iterations of OpenAI models. Note that you can opt out of your data being stored and/or used for training, on both the web and mobile versions of ChatGPT.

Similarly, Google’s Bard stores your conversation data for up to 18 months by default. Human reviewers read and annotate conversation data to improve future iterations of the model, so you should never disclose confidential or proprietary information. You can choose to delete Bard conversation history in your Google Account settings, but even with this option, human reviewers will see the depersonalized conversation data.

### Best Practices

Before you use generative AI tools for work, familiarize yourself with your company’s generative AI policies. Different companies have different policies surrounding the use of these tools. Some companies, including Amazon, Wells Fargo, and Deutsche Bank have outright banned the use of ChatGPT for company work.

Other companies may have more flexible policies regarding generative AI tools. If your company allows you to use tools like ChatGPT for work, you should still follow some best hygiene practices. Make sure not to copy sensitive or proprietary company information into the tool. If using ChatGPT, you may also want to select the “Turn off chat history” option so your conversation history isn’t used to train OpenAI models. Overall, never assume that your conversation history is private. 

## Bias

AI systems are susceptible to bias. When AI models are trained on discriminatory training data, the models reflect and magnify these biases at scale. These biases can have very real, negative consequences on people, such as disadvantaging job applicants from underrepresented backgrounds or skewing results from predictive diagnostic healthcare algorithms. As more AI systems are used across industries, from healthcare to education, it’s critical to be aware of potential bias – both when developing and evaluating models.

AI systems have several sources of bias including: **training data** bias, **algorithmic** bias, and **cognitive** bias. If you are developing in-house generative AI systems, it’s important to be aware of these possible avenues for bias. 

**Training Data Bias**

In training data, overrepresented or underrepresented groups can introduce bias. Google’s hate-speech detection algorithm Perspective is reported to exhibit bias against certain groups, including black American speech patterns. The training data did not include sufficient examples of typical black American linguistic patterns, leading the model to flag certain slang as toxic. Leading generative AI companies like OpenAI and Anthropic still use Perspective to determine the toxicity of their LLMs, which can perpetuate these biased predictions.

**Algorithmic Bias**

Algorithmic bias can be caused by unfairly weighting certain factors in algorithm decision-making. Prior research has shown that black patients assigned the same level of risk as white patients by a widely used health score algorithm were sicker, on average. In this case, the bias can be attributed to the algorithm’s use of health costs as a proxy for health needs. Since less money is spent on black patients who have the same level of need, the algorithm falsely concluded that black patients were healthier than equally sick white patients.

**Cognitive Bias**

Cognitive bias arises from the people who process and make judgments from the results of AI systems. In its report *Towards a Standard for Identifying and Managing Bias in Artificial Intelligence*, NIST noted that “human and systemic institutional and societal factors are significant sources of AI bias as well, and are currently overlooked. Successfully meeting this challenge will require taking all forms of bias into account” 

### Mitigating Bias

Although extensive research has been conducted about how to best mitigate bias in AI systems , there is still no clear-cut solution. However, there are steps you can take.

If you are training generative AI systems in-house, strive to acquire or compile training data that is as large and diverse as possible. You can also carefully monitor error rates and identify when performance deteriorates for certain groups or subsets of the population. During the model development phase, you can take mathematical approaches for de-biasing, such as [adversarial de-biasing](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7611652/) or [oversampling](https://link.springer.com/article/10.1007/s10115-011-0463-8). During model evaluation, you can assess how well the model makes predictions for independent groups. This can help you validate how the model generalizes to data across groups, providing insights on potential bias that is introduced during the modeling step. Finally, in deployment, recognize that bias can occur when in-practice data differs from training data. To identify such bias, it’s crucial to monitor AI system performance after deployment for any regressions or errors in performance.

## Spearphishing Attacks

Phishing is currently the most prevalent form of cybercrime, with over a trillion phishing emails sent per year. **Spearphishing** is a type of phishing that targets specific individuals, often those with privileged access to systems. Although spear phishing campaigns made up only 0.1% of all email-based phishing attacks in 2022, they were responsible for 66% of all breaches.

Generative AI tools like ChatGPT, Bard, and Bing can allow attackers to create highly personalized and convincing phishing emails, based on publicly available information. Attackers can automate social media web-scraping algorithms to collect data about targets, creating knowledge graphs about their personal lives. By feeding this data into an LLM, they can generate spearphishing messages complete with well-crafted personas

### Common Defenses

- Phishing Awareness Training
- MFA
- Generative AI Dewtection Measures

Generative AI can improve spearphishing detection by predicting the intent of messages. First, LLMs can be used to generate large, varied datasets of emails to train models on to recognize different kinds of intent. This can be less time and cost-intensive than the traditional model training process of acquiring vast amounts of human-labeled emails.

In addition to message intent, models can also be trained on signals of sender intent. If we establish a behavioral baseline for known senders or groups of senders, deviation from observed history could indicate a potential phishing attack. As generative AI is used to develop more convincing phishing attacks, organizations should be quick to develop their own generative AI systems to combat these dangers.