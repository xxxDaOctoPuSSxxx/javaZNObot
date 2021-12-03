# Deployment Part of Project #

* __Don't do in this part of code any changes or if you need some changes contact to @UzunDD__
* __Requirements:__

  1 Install Linux or enter on VM with Linux via SSH

  2 [Install AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html) and configure credentials in file .aws (insert access key & secret key with programmatic administation permissions);

  3 Inatall [TERRAFORM_VERSION: "1.0.9"](https://learn.hashicorp.com/tutorials/terraform/install-cli?in=terraform/aws-get-started) & [TERRAGRUNT_VERSION: "0.35.6"](https://terragrunt.gruntwork.io/docs/getting-started/install/#install-terragrunt) or latest;

  4 Visit [AWS Console](https://aws.amazon.com/console/?nc1=h_ls) in [System Managment / Parameter Store](https://eu-central-1.console.aws.amazon.com/systems-manager/parameters/) in region what you need to deploy & enter sensitive data (Github access token, Telegram bot token);

  5 [Clone repository with project](https://github.com/xxxDaOctoPuSSxxx/javaZNObot) for automatic deploy change directory to __deployment > enviroments >__ (set enviromet what you need to deploy __cd to__) __development / testing__ or __production server__;
  
  6 In terminal RUN command __terragrunt run-all plan__ to check what resources terraform must create in AWS & then RUN command __terragrunt run-all apply__, to create infrastucture  for Java telegram ZNO bot;

  7 To learn more how deploy build project read about project [__Code Build__](https://github.com/xxxDaOctoPuSSxxx/javaZNObot/blob/main/deployment/terraform-modules/codebuild/readme-code-build.md)!
