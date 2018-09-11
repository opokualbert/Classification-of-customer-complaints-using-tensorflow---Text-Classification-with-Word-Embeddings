# Classification of customer complaints using tensorflow - Text Classification with Word Embeddings
In this post, I show how to classify consumer complaints text into these categories: Debt collection, Consumer Loan, Mortgage, Credit card, Credit reporting, Student loan, Bank account or service, Payday loan, Money transfers, Other financial service, Prepaid card.

This kind of model will be very useful for a customer service department that wants to classify the complaints they receive from their customers. The classification of the issues they have received into buckets will help the department to provide customized solutions to the customers in each group.

This model can also be expanded into a system, that can recommend automatic solutions to future complaints as they come in. In the past, performing these kinds of tasks were done manually by multiple employees and of course, take a long time to accomplish, delaying swift response to the complaints received.

Machine learning and AI are here to solve this caliber of problems. Imagine you can classify new complaints with 95% accuracy and route them to the right team to resolve the issue. That will be a win and time saving to any business. Your customers will be happy because the right expert from your business will talk to your customers in trying to resolving their complaints. This will translate into lowering churning rate which means more revenue.

I trained a text classifier with 66,806 of data on customers that have made a complaint to consumer financial protection bureau - CFPB about US financial institutions on the services they have rendered to these consumers. The dataset is on kaggle.com at this link https://www.kaggle.com/cfpb/us-consumer-finance-complaints.

I used the universal-sentence-encoder-large/3 module on the new tensorflowhub platform to leverage the power of transfer learning which according to Wikipedia, is a research problem in machine learning that focuses on storing knowledge gained while solving one problem and applying it to a different but related problem. Google and other teams have made available on tensorflowhub, models that took them about 62,000 GPU hours to train for our free use.

This dataset is relatively not large but this kind of machine learning process requires more compute power so I chose to use Google’s colab, which gives the option to train a model with free GPU. I have a previous blog post on downloading Kaggle datasets into Google Colab on my [website](https://opokualbert.com/post.html), you may want to check it out if you are interested in downloading this dataset to follow along with this demo.

I will walk through the steps and in the end, we will classify new complaints and see how the model performed.
