To define a workflow, we need to define workflow json.


## Workflow Testing


1. First, the workflow needs to be deployed on the conductor server. To deploy the workflow json, we can either: <br>
  a. Access the swagger console -- `http://localhost:8080/swagger-ui/index.html#/`  <br>
      Under `metadata -> resource`, look for `POST /api/metadata/workflow`
     ![image](https://github.com/anushkadeshpande/conductor/assets/53345232/635b144e-f4c3-4796-bb06-5ebebd34e230)

OR

   b. Make a REST call to the endpoint -- `http://localhost:8080/api/metadata/workflow` and pass the workflow json as payload


2. To check your workflow, go to Definitions on the Conductor UI and select your workflow. <br>
Here, workflow definition can be checked via the flow diagram
![image](https://github.com/anushkadeshpande/conductor/assets/53345232/7b809423-f0b6-44c8-809b-5465b936bd1a)

3. Next, to execute a workflow, go to workbench, select your workdlow name, version and add the input json and then execute it <br>
After that, clicking on the Execution Id will bring us to this page where one can check the input, output, logs, etc

![image](https://github.com/anushkadeshpande/conductor/assets/53345232/bce0b184-fd5a-48a3-98e2-1ba8c50c6982)

