# 03_01 AWS CodePipeline and CodeBuild
CodePipeline and CodeBuild are tools for implementing CI/CD in Amazon Web Services.  

- With [CodePipeline](https://aws.amazon.com/codepipeline), developers can model the stages of their pipeline and the actions that need to be taken in each stage.  
- [CodeBuild](https://aws.amazon.com/codebuild) provides an on-demand build service that can be used with CodePipeline to implement the steps needed to build, deliver, and deploy code.

## Recommended Resources
- [DevOps with AWS](https://www.linkedin.com/learning/devops-with-aws): Covers AWS automation services including CodeBuild and CodePipeline.

## Prerequisites
Having the following items in place before starting this lab will help you have a smooth experience.

1. A [GitHub account](https://github.com/join) is required to host the code for the sample application.
1. An [Amazon Web Services account](https://aws.amazon.com/free) is needed to deploy the sample application used for the deployment target.
1. The sample application should be in place before starting.  See [00_06 About the Exercise Files](../../ch0_introduction/00_06_about_the_exercise_files/README.md) for steps to deploy the sample application.
1. The exercise files for the course should be downloaded and accessible on your local system.

## Implement the Experimental Pipeline
To implement the experimental pipeline in AWS CodePipeline and CodeBuild, you will need to create a GitHub repo, add the exercise files, and modify the files for your project.

Then you'll add the service account credentials.  Next, you'll create the project that implements the pipeline.

And finally, you'll trigger the pipeline to deploy the sample application.

Before starting these steps, open the Output tab of the Cloudformation stack for the sample application.  You'll be referencing values displayed on that tab.

### 1. Create a GitHub repo for the sample application code
Because this course covers multiple tools, a dedicated repo is need for each tool to prevent unexpected deployments to the sample-application.

#### 1.1 Create a repo and upload the exercise files for this lesson
1. Create a new GitHub repo. Give the repo a name and description.  Please select **Public** for the repo visibility to simplify access.  Select the option to add a README file and select **Python** when adding a `.gitignore` file.
2. From ther repo home page, select **Add file -> Upload files**.
3. Select **choose your files** and browse to the exercise files for this lesson on your local system.
4. Select all of the files and then select **Open**.
5. After the files have been uploaded, enter a commit message and select **Commit changes**.


TODO: UPDATE

- https://docs.aws.amazon.com/codebuild/latest/userguide/build-env-ref-env-vars.html

- CodePipeline should use the Zip format, not the clone format


- https://docs.aws.amazon.com/codebuild/latest/userguide/build-spec-ref.html

- attach the policy to the role created by codebuild

- https://aws.amazon.com/codebuild/pricing/
- https://aws.amazon.com/codebuild/pricing/

