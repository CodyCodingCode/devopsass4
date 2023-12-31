# devopsass4

CI/CD Pipeline Setup
AWS CodePipeline:

Go to AWS CodePipeline and create a new pipeline.
Connect it to your Git repository.
Configure a source stage to detect changes in the repository.
AWS CodeBuild:

Set up a build stage in CodePipeline.
Create a buildspec.yaml file in your repository to define build steps.
Configure CodeBuild to use this buildspec.yaml during the build stage.
Automated Tests (Optional):

If applicable, include automated tests in the buildspec.yaml.
Configure CodeBuild to run tests during the build stage.
AWS CodeDeploy (Deployment):

Add a deployment stage to your CodePipeline.
Choose S3 as the deployment provider and select the S3 bucket where you hosted your website.
Set up the deployment configuration.

AWS CodeBuild:
Set Up CodeBuild:

Open the AWS Management Console.
Navigate to the CodeBuild service.
Create a New Build Project:

Click on the "Create build project" button.
Configure Build Project:

Project Name:
Enter a name for your build project.
Source:
Choose "AWS CodePipeline."
Select the CodePipeline you created earlier.
Environment:
Choose the runtime environment for your build (e.g., Ubuntu, Node.js, etc.).
Buildspec:
Select "Use a buildspec file" and enter the buildspec file location (e.g., buildspec.yaml).
Artifacts:
Choose the type of artifacts to be produced by the build.
Click "Create build project."
Create a Buildspec.yaml File: