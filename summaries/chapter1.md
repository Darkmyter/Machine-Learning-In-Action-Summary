# What is machine Learning Engineering

ML engineering focus on creating system that around the complex work of different specialists (Data Scientist, Data Engineers, Business unit, ...). With the use of tools, process and methodology, the aim is to build a system that is scalable, maintainable and minimizes the chances of abandonment and work need to solve the business problem with the accuracy proven to provide.

ML Engineering road map is the process and methodologies that guide the design of the product to prevent rework, confusion and complexity.

ML Engineers need to be proficient in data science, traditional software engineering and project management.


<p align="center" width="100%">

| <img width="75%" src="resources/ch1-ml-road-map.png"> | 
|:--:| 
| *ML Engineering road map for project work* |
</p>


## Why ML projects fail ?
Understanding why most ML projects fail is equally important as iterating through the steps of the road map. Learning from past experiences of others is important in this field.

<p align="center" width="100%">

| <img width="75%" src="resources/ch1-why-ml-projects-fail.png"> | 
|:--:| 
| *Estimation of why ML projects fail* |
</p>

In general, failures are due to:
* The inadequacy of the DS team in terms of experience or size in relevancy to the problem scale.
* Misunderstanding of the business goals:
  * lack of detail in project expectations
  * miscommunication owing to the challenging technical complexity.
* Relative industry immaturity in tooling.



<p align="center" width="100%">

| <img width="75%" src="resources/ch1-ml-project-detours.png"> | 
|:--:| 
| *ML project detours that lead to project failure* |
</p>

## The core principles os ML Engineering
An introduction of the tents of ML Engineering and their problematic side.
### Planning
The planning phase needs to focus on **what will be built** and **why it needs to be built**. Putting aside the technical details and the **how it will be built question** by the DS team, help keep the attention of understanding the need, expectations and the end goal of the predictions.


<p align="center" width="100%">

| <img width="75%" src="resources/ch1-planning-discussion-diagram.png"> | 
|:--:| 
| *ML project detours that lead to project failure* |
</p>


### Scoping and research
When it comes to research, two problematic mindsets exist:
* "Applicative ML", where engineers perceive ML as tools to solve the business problem.
* "Research ML", where engineers, and mostly academics, focus on innovation and discovery to advance the knowledge and research in ML field.

The first mindset might content its research to a brief reading of blogs and similar problems posted online and identify a solution that it simple with short delivery time. This could lead to oversight the true challenges of the problem and delivering under-performing solution.

The second mindset would go through a meticulous research phase, identify an advanced solution that was well studied. However, the solution is often too complex to deliver in the expected time or would require a big deal of resources.

Finding the a middle ground between these two mindsets is key.

### Experimentation
Experimentation can go wrong if:
* The team patches together a quick solution that does not deliver and thus  erodes the trust and faith put in the team, along with money.
* The teams loses track of time, running multiple experiments and blows through the budget resulting the cancellation of the project.

### Development
Building a code base involves multiple people adding changing the code daily. Having no development practices and poor deign can make the code break easily and be hard to improve with no features.

A moduralized code base is must have for easier collaboration on projects.

### Deployment

Deployment of models needs to strive for simplicity and good budget estimation.  
Ovoid underpowered strategies that render the predictions useless and overpowered strategies that burn money.

A couple deployment elements at different costs:
* **Prediction / Inference:**
  * **low cost:** offline training, offline serving
  * **high cost:** Active retraining, online serving
* **Prediction / Inference volumes:**
  * **low cost:** OLTP (table storage) batch predictions in KB-MB range
  * **high cost:** NoSQL/REST/edge Millions of predictions per day
* **Training / implementation complexity:**
  * **low cost:** Small data, simple model, minimal feature engineering
  * **high cost:** Extremely large data, ensembles, computationally complex model
* **Drift volatility:**
  * **low cost:** Relatively static, retraining on a scale of months
  * **high cost:** High concept / feature drift, retraining < every hour

### Evaluation
Evaluating the impact of the model on the business side is fundamental to the project survival and need to be performed prior to deploying it to production.  
A/B testing and statistical models are the tool to tie the model to the business revenues.

## The goal of ML Engineering
The goal of ML Engineering goes back to the simple task of solving a problem. It can be mistaking, by enthusiasm, as creating a fancy solution or creating the most impressive research paper.  
This problem is solved with statistics, algorithms and predictive models because their are difficult, monotonous or error-prune to be done by humans.  
Keeping in mind the methodology of ML projects helps overcoming their complexity and possible failure.

<p align="center" width="100%">

| <img width="75%" src="resources/ch1-ml-methodo-map.png"> | 
|:--:| 
| *ML project methodology component map* |
</p>