# Breakthrough-Tech-AI
Final writeup for Involve.AI project

**The Problem:**
Potential customers who visit the Involve.AI website might not be familiar with AI and not very convinced to move forward with buying into their services. They see statistics and promises of what they could get without getting to see a free demo before buying in.

**The End Goal:**
Our goal was to create a widget on the Involve.AI website that would allow the potential customer to have a small taste of AI's capabilities. The customer can input some publicly available data into a ML model and quickly receive some general results to see the AI in action. The results of the model would be very general but it would give the potential customer an idea of what they would be paying for and be more likely to move forward with Involve.AI.

**Models and Data:**
The models we used were pre-trained by Involve.AI and our task was to observe its performance on a new domain. The models were previously trained on emails, but we wanted to see their performance on company/product reviews. These datasets were publicly available by G2 Crowd and given to us by Involve.AI. In order to improve model performance, we applied various pre-processing techniques to clean the data.

The models performed generally well. The models were trained using unstructured text, which is the same case for reviews so we did not have to modify the models themselves. The models used named entity recognition to pick up keywords from the unstructured text to provide a final label for the subject of the text. This allows an easy categorization of what various reviews are discussing. We also incorporated a sentiment analysis score, which depicted whether a certain review contained a positive or negative tone. This is helpful for companies since they could have a quick glance at how customers feel about their products/services.

**Deployment:**
Once we created a pre-processing script, we transitioned to working on the deployment for the website widget. We used Apache Airflow and AWS Lambda to invoke the correct system calls once the customer clicks the widget to try out the demo model. 

**Ending Note:**
This project with Involve.AI was a great experience, it was unlike any other school assignment I have worked on. In the early stages of assessing model performance, we were not given clear metrics on how to do so. We had lots of discussion with our challenge advisor about our different ideas for experimentation. This is completely different from school where there is a clear rubric for every assignment and there is distinct right or wrong way to do something.

I had a fantastic learning experience while working on a real problem with industry professionals. I am grateful to Involve.AI and Breakthrough Tech for this opportunity and I hope more students get a chance to participate in this type of program because the experience was priceless.
