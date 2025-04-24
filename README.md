<br/>
<p align="center">
  <a href="https://github.com/Antovex/Portfolio-AutoDeploy">
  </a>

  <h1 align="center">Portfolio-AutoDeploy</h3>

  <p align="center">
    Files deployed as soon as pushed
  </p>
</p>



## About The Project

This project is an application of the real life based scenario. In this when a developer pushes file to the master/main branch of repository, Github Action gets triggered automatically. The action then performs a job, which pushes the updated code to a particular S3 bucket. Hence the deployment becomes seamless and saves time of developer.
<p align="center">
</p>

## Architecture
<p align="center">
<img src="https://github.com/Antovex/Portfolio-AutoDeploy/blob/main/Architecture/Portfolio_AutoDeploy_Architecture.png?raw=true" width="600" height="400">
</p>

## Getting Started

You just need a laptop with an internet connection, a code editor and git installed for this project and it will be completed within just few clicks.

### Prerequisites

* Make sure you have an active AWS account (Free tier will also work).
* Your website files.

### Project Setup

1. [Make a S3 bucket with public access](https://saturncloud.io/blog/how-to-make-an-s3-bucket-public/) available (Give it a unique name).

2. [Make a new Public repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/quickstart-for-repositories), and go to Actions tab.

3. Click on "[set up a workflow yourself](https://resources.github.com/learn/pathways/automation/essentials/building-a-workflow-with-github-actions/)".

4. Copy and paste the yaml file from this repositories "[/GithubAction_file/main.yml](https://github.com/Antovex/Portfolio-AutoDeploy/blob/main/GithubAction_file/main.yml)".

5. Specify main/master branch, your preferred AWS region and your AWS bucket name.

6. Go to your AWS account and [create new AWS secreat key which has AWS S3 full access](https://supsystic.com/documentation/id-secret-access-key-amazon-s3/).

7. Go to Settings=>Secrets and variables=>Actions then create 2 "New repository secret" named as AWS ACCESS KEY ID (put ID) and AWS SECRET ACCESS KEY (put the value).

8. Now commit this change for now.

9. Now push the website files to that github repository in which you just made the actions files.

10. Go to your S3 bucket, click on the bucket name, then go to properties, scroll till the last and turn on [Static Hosting](https://docs.aws.amazon.com/AmazonS3/latest/userguide/WebsiteHosting.html) option and mention "index.html".

11. Now you will get a link for website, and we can view our website.

12. Now from the next push, the changes will be deployed automatically. 

## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.
* If you have suggestions for adding or removing projects, feel free to [open an issue](https://github.com/Antovex/Portfolio-AutoDeploy/issues/new) to discuss it, or directly create a pull request after you edit the *README.md* file with necessary changes.

### Creating A Pull Request

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AddedFeature`)
3. Commit your Changes (`git commit -m 'Add some AddedFeature'`)
4. Push to the Branch (`git push origin feature/AddedFeature`)
5. Open a Pull Request

## Author

* **Antarin Ghosal** - *IT Student* - [Antarin Ghosal](https://github.com/Antovex)
