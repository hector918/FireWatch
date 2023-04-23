## Inspiration

Our inspiration for FireWatch came from how unprepared most communities are when it comes to the impacts of wildfires, a destructive side effect of our rapidly declining climate. The devastating impacts of wildfires on our climate and communities is a clear indication of how important it is to address them. Due to the increasing frequency and intensity of wildfires, there is a critical need for innovative solutions to help mitigate their impact. FireWatch was created with the goal of addressing this need by predicting wildfires before they have the chance to occur and spread. We believe that FireWatch has the potential to combat one of the most destructive side effects of climate change. As the theme of the hackathon is climate, we wanted to promote climate resilience by providing users with essential information that can help them stay informed and potentially save lives.

## What it does

FireWatch is an artificial intelligence-powered wildfire prediction and mitigation system with a user-friendly interface geared towards people like forest rangers, firefighters, emergency response teams, property owners, and government officials who stay prepared and respond proactively to wildfires. We have built and trained two advanced machine learning models that analyze images to generate predictions on the chances of a wildfire occurring. Our AI chatbot finishes our product, making it a true personalized and end to end solution. We leveraged the power of AI to take the data from our other two machine learning models and analyze it to provide the user with personalized feedback on their wildfire risk and wildfire prevention.

FireWatch provides users with the following features: 

Wildfire Risk Prediction: Firewatch uses satellite imagery to predict the likelihood of a wildfire occurring in a specific area. By analyzing environmental factors present in satellite imagery and data, FireWatch generates an accurate wildfire risk score. 
Personalized guidance and Support With Wildfire Prevention: FireWatch can provide users with preventative measures that can be taken to minimize the risk of a wildfire based on their wildfire risk score and other data through an AI chatbot. FireWatch can provide recommendations on evacuation plans, government guidelines on preventing wildfires, contact information for local fire departments and emergency services, and information on clearing flammable materials from around properties. The bot can also answer questions about wildfires and provide additional information on how to prevent wildfires.
Secure Authentication System: FireWatch also has a secure authentication system that ensures the safety of user data. We used an SQLite database to store user data and make our authentication system. All sensitive user information is securely encrypted with Argon2. 
User-Friendly Interface: FireWatch provides a user-friendly interface that is easy to navigate. All users can swiftly access information on their wildfire risk and take action to protect themselves, maximizing the utility of our platform.

## How we built it

FireWatch was built utilizing a collection of languages and technologies. We used languages such as Python, HTML, CSS, and JavaScript and technologies like Flask, AJAX, TensorFlow, Keras, OpenAI, AutoGluon, SQLite, Leaflet in the development of our website. HTML, CSS, and JS were used in the front end and the Flask python framework was used in the backend. AJAX was used to handle communication between the front and back ends. We built our secure authentication system with an SQLite database to store user data and HashLib and Argon2 to ensure security. FireWatch uses the Leaflet JavaScript library to provide a map where users can select the location they want to survey for wildfire risk. From there, the longitude and latitude coordinates are extracted from the location chosen and fed to both of our advanced machine learning models. We built our first machine learning model by leveraging AutoGluon and about 50,000 instances of wildfire related satellite imagery extracted from the Wildfire Prediction Dataset (Satellite Images) Dataset to train a convolutional neural network, or CNN, to efficiently identify wildfire risk from satellite imagery alone. With this model, we can take in coordinates anywhere in the world, and use satellite imagery in conjunction with our model to accurately predict wildfire risk. We built our second machine learning model by leveraging TensorFlow, Keras, and data augmentation along with about 100,000 instances of data collected about wildfires by satellites present in the DeepSat (SAT-4) Airborne Dataset to train another CNN to identify different types of terrain and the wildfire risk associated with them. With this model, we can take in coordinates anywhere in the world, and analyze land using data collected by satellites to provide insight into wildfire risk and prevention. After the satellite imagery associated with the coordinates are analyzed by our machine learning models to generate a wildfire risk score and other data, users can navigate to our AI chatbot, who is aware of the wildfire risk and other data involved. The chatbot provides the user with the likelihood of a wildfire occurring in their area, and will proceed to give them recommendations on the preventative measures they can take to stop a wildfire from happening in their area. The user can talk with the chatbot for further clarification or confirmation.

## Challenges we ran into

We faced numerous challenges during the creation of FireWatch. The main challenge we faced while creating FireWatch was training accurate machine-learning models to analyze satellite data and imagery. Finding the perfect datasets and training the model was very time consuming as it took almost 4 hours to train both models due to their complexity and the sizes of the training datasets. In addition, the validation accuracy of our models were quite low at first, however we were able to improve the validation accuracy from 55% to 99% by adding more layers and complexity to our models. Another challenge we faced was communication. Although our team has worked together several times in the past, ClimateHacks was our first online hackathon, which showed in our communication. It was difficult to cooperate as we were all working from different places and faced technological limitations due to working remotely, which meant that we were not able to focus on our projects for long stretches of time. One final challenge we faced was integrating our chatbot into our website. Figuring out communication between the front and back end, as well as figuring out how to factor the outputs from our machine learning models into the final response from the AI chatbot were both challenges that we were eventually able to overcome. Overall, ClimateHacks was a learning experience for everyone on our team.

## Accomplishments that we're proud of

We have accomplished a lot throughout the creation of FireWatch. The first thing we are proud of is creating two accurate neural networks capable of analyzing large amounts of data and trained by a large datasets under the time constraints presented by this hackathon. We are also proud of the potential real world implications that FireWatch may have. We recognize that FireWatch has the potential to save lives and people’s properties that may be important to them. One final thing we are proud of is managing to build a useful and functional product in our first online hackathon. This challenged our communication skills as a team, but we are proud that we were ultimately able to communicate with one another and finish this project. 

## What we learned

We learned many things throughout the process of building FireWatch. While we were training our models using machine learning, we were able to expand our knowledge by using many different datasets and many different ways for the model to interpret the data that it’s receiving from the user. We also were able to expand our knowledge on Flask and AJAX requests by using JavaScript and an interactable map which sends information from the frontend to the backend. Throughout the project, we researched and analyzed the causes and potential risks of wildfires and were able to find ways to predict and prevent them. Overall, we worked as a team and were able to learn many new things throughout the creation of FireWatch.

## What's next for FireWatch

We are ambitious about the future of FireWatch. We plan to improve and expand FireWatch’s capabilities by expanding the range of environmental factors we will take into account when helping with wildfire management. We will also train new, more powerful machine learning models that will take this expanded range of environmental factors into account to make more accurate predictions about wildfire probability. We also plan to allow users to sign up to be alerted to possible wildfires in their area, which will help them be prepared to deal with a potential wildfire in their vicinity. We also plan to create a mobile app for FireWatch to allow users to access FireWatch from their smartphones. This will allow users to receive real time updates and alerts pertaining to wildfires near them, increasing the utility of our app. Lastly, we are committed to continuously improving FireWatch’s user experience by implementing user feedback and conducting regular user testing. This will ensure that FireWatch remains user-friendly, accessible, and useful for all users. Overall, we plan to make FireWatch a more accessible and powerful platform to help reduce the devastating impacts of wildfires.
