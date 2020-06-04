# APAC Machine Learning TFC Training
This is a collection training resources used for new TFC members. The original git hub repository is [here](https://github.com/glyfnet/apac-tfc-training).

## Setup
1. Request GPU limit increase 
    
    For the CV1 lab, we will be using GPU SageMaker notebook instances. You will need to request a limit increase +1 for a p2 instance.

    Instructions for limit increase are [here](Setup.ipynb).

2. Download the cloudformation template

    Download the cloudformation template [here](/../../raw/master/mlu_computer_vision.yaml) right click 'Save As' and download the cloudformation template.

    **Note** Make sure you save the file as a .yaml file.

3. Create a new cloud formationstack

    In another browser window or tab, login to your AWS account. Once you have done that, open the link below in a new tab to start the process of deploying the items you need via CloudFormation.

    [![Launch Stack](https://s3.amazonaws.com/cloudformation-examples/cloudformation-launch-stack.png)](https://console.aws.amazon.com/cloudformation/home#/stacks/new?stackName=APAC-TFC-Training)

    **Note** You may need to select the region where the p2 instance is available.

4. Upload the cloud formation template

    Select `Upload a template`,  click `Choose file` and select the cloudformation template file you've just downloaded and then click `Next`.

5. Configure stack options

    All of the defaults in this section will be sufficient to complete the lab. If you have any custom requirements, please alter as required. Once you're done, click the `Next` button to continue.

    Finally, in the next section, scroll to the bottom of the page and check the checkbox to enable the template to create IAM resources and click the `Create stack` button.

6. Launch SageMaker Notebook

    To begin the lab, go to SageMaker -> Nootebook Instances and click on Notebook instance and open the `tfc-training` notebook (or the name of the notebook you provided in Cloudformation).

    You should see all the course notebooks pulled from the git repo.

## Courses
Follow the links below to begin one of the courses.

* [Computer Visions 1](Computer_Vision_1)

* [Natural Language Processing 1](Natural_Language_Processing_1)
