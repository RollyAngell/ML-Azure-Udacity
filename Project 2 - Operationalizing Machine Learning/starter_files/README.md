*NOTE:* This file is a template that you can use to create the README for your project. The *TODO* comments below will highlight the information you should be sure to include.


# Your Project Title Here

*TODO:* Write an overview to your project.

## Architectural Diagram
*TODO*: Provide an architectual diagram of the project and give an introduction of each step. An architectural diagram is an image that helps visualize the flow of operations from start to finish. In this case, it has to be related to the completed project, with its various stages that are critical to the overall flow. For example, one stage for managing models could be "using Automated ML to determine the best model". 

![Arquitectura](https://user-images.githubusercontent.com/8076356/107143883-74302f80-6905-11eb-8a6a-ff6955193748.png)

## Key Steps
*TODO*: Write a short discription of the key steps. Remeber to include all the screenshots required to demonstrate key steps. 

## STEP 1: Authentication

### AZ Configuration

![image](https://user-images.githubusercontent.com/8076356/107144070-a2623f00-6906-11eb-8bb2-f009e2a86737.png)

*We can see all properties*

![image](https://user-images.githubusercontent.com/8076356/107144094-cc1b6600-6906-11eb-9d06-f5469c5d3034.png)

*AZ login*

![image](https://user-images.githubusercontent.com/8076356/107144105-e1909000-6906-11eb-88f8-171b0c0db179.png)

*az extension add -n azure-cli-ml*

## STEP 2: Automated ML Experiment

### 2.1. Registered Datasets
Here we upload the bank marketing dataset.

![image](https://user-images.githubusercontent.com/8076356/107144668-b0b25a00-690a-11eb-8a53-8f8ddf75a690.png)

*Uploadin dataset*

![image](https://user-images.githubusercontent.com/8076356/107144274-1cdf8e80-6908-11eb-9f59-2d0876e5f8aa.png)

*We can see 2 dataset  and we use firts*

### 2.2. Completed experiment

![image](https://user-images.githubusercontent.com/8076356/107144744-3b935480-690b-11eb-8383-242538bcd9ef.png)

*We run a Automated ML with classification task.*

![image](https://user-images.githubusercontent.com/8076356/107144783-74cbc480-690b-11eb-8550-85307cd7afd5.png)

*Completed experiments*

![image](https://user-images.githubusercontent.com/8076356/107144797-88772b00-690b-11eb-87c3-4255cace6035.png)

*Detail of the experiment*

### 2.3. Best Model

The best model was Voting Ensemble

![image](https://user-images.githubusercontent.com/8076356/107144822-b6f50600-690b-11eb-9905-2d7847d566b4.png)

![image](https://user-images.githubusercontent.com/8076356/107144839-d3913e00-690b-11eb-9d86-8948a446aa7f.png)


## STEP 3: Automated ML Experiment

### 3. Deploy the best model
In this step, the best model from the AutoML run, Voting Ensemble, was deployed using Azure Container Instance.

### 4. Enable logging
In this step, logging was enabled with a Python script and the Application Insights page could be used to monitor the app.

### 5. Check swagger documentation
In this step, swagger ui was used to see the input required for an API request in order to obtain predictions from the deployed model. Two modes of API requests were seen, i.e. GET and POST.

### 6. Consume model endpoint
After finding out the json structure of the input, in this step a Python script was run to get the prediction from the endpoint by sending the new data in the required input structure.

### 7. Create, publish, and consume a pipeline
After the model was deployed, a pipeline was created and publish to ease duplicating the project flow. Another run was scheduled and eventually re-run.

Completed pipeline run:

## Screen Recording
Link of youtube

https://youtu.be/d8ScC-0NhUE

## Standout Suggestions
*TODO (Optional):* This is where you can provide information about any standout suggestions that you have attempted.
