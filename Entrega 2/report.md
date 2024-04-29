## Deployment plan

We propose to make the model accessible through a public website. Specifically, the site will allow to enter the basic information of a news item and determine its veracity. We expect to be able to deliver a reasonable verdict for the different news items and to include the necessary information about the system to avoid misunderstandings.

To achieve this it will be necessary to deploy a web site (frontend) that will act as an interface and an api rest that will control access to the model. 

- We plan to build the frontend with nextjs and deploy it on a platform like vercel or netlify.

- Regarding the API (backend), we plan to implement it with python giving continuity to the code produced until this deliverable. However, it will be necessary to add a framework like fastApi, django or flask in order to expose the endpoint. This endpoint will be the access point to a module that actually contains the model and provides the classification service. To avoid having to go through the training process every time a request is made we will make use of joblib; this library allows to serialize the state of the model once a single training is completed. In this way, the requests can be answered in decent times by loading the stored model. Finally, when adjustments are needed, the new model can be trained and the same mechanics can be followed.

We consider this structure adequate because it is decoupled. That is, it allows us to scale the components independently. For example, we could modify only the model and use the same web interface, modify the look and feel of the interface without affecting the future by allowing direct access to the classifier via the API without having to make significant changes to the other components.  

## Analysis of initial impacts

The impacts that a solution that allows determining the veracity of a news item from its content and the most basic information (such as the title and date of publication) may have are as follows:

### Ethical aspect

Training can introduce biases, this is an inherent effect of training data, which after all is of human origin. It is critical to ensure that training data are diverse, representative, and from reliable sources. For example, manipulating the labels could lead the model to label as false relevant information that is intended to be censored or downplayed.

### Social impact

If our solution is used correctly, it can increase public trust in the news by verifying authenticity. That is, reducing misinformation and several of its effects such as polarization.

### Legal aspects:

As part of the deployment we must ensure that we expose important information. For example, how decisions are made and what are the limitations of the system, so that it is understood that it is not an infallible mechanism and that possible mistakes do not correspond to bad intentions in the training of the model but to the inherent error that all forms of artificial intelligence present and try to minimize. 

On the other hand, there may be an impact on the handling of personal or non-rights-free data. To this end, care must be taken to avoid unauthorized disclosure of information and to use free or properly licensed content. 

### Economic impact

A trusted solution can attract users and organizations seeking to verify the authenticity of news. Sustaining such solutions involves updating the model so that it remains competent in its classification task. So it is possible to generate a business model around it.

### Conclusion

The development of a web service to identify true or fake news has the potential to be a valuable tool in the fight against disinformation. However, it should be implemented with caution, considering the possible ethical, social and legal impacts, and ensuring the transparency and accuracy of the system. In addition, it is important to complement this service with media literacy programs to empower users to evaluate information for themselves.
