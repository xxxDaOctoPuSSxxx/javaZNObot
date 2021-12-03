# Code Build #

After RUN __terragrunt run-all apply__ terraform will create template infrastructure and begins from [__init-build__](https://github.com/xxxDaOctoPuSSxxx/javaZNObot/blob/main/deployment/terraform-modules/init-build/readme-init-build.md) module.

In __Code Build__ module is inserted variables from terragrunt.hcl file and automatic detect webhook from GitHub. If trigger detected Code Build cloned repository, check infrastucrure, rebuild docker image, push them to ECR, create new taskdefinition for ECS and our changes in application will be running on all cluster nodes.
