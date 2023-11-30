# <p align="center">Send the contributor an email when the PR is merged</p>

<p align="center">
  <a href="https://discord.gg/ccZn9ZMfFf">
    <img src="https://img.shields.io/badge/chat-Discord-7289DA?logo=discord" alt="flows.network Discord">
  </a>
  <a href="https://twitter.com/flows_network">
    <img src="https://img.shields.io/badge/Twitter-1DA1F2?logo=twitter&amp;logoColor=white" alt="flows.network Twitter">
  </a>
   <a href="https://flows.network/flow/createByTemplate/send-thank-you-email-to-contributor">
    <img src="https://img.shields.io/website?up_message=deploy&url=https%3A%2F%2Fflows.network%2Fflow%2Fnew" alt="Create a flow">
  </a>
</p>


[Deploy this function on flows.network](#deploy-pr-merge-notifier-on-your-github-repo), and you will automate the work to get reach out to the contributors. When the Pull Request is merged by maintainers, send a thank-you email to the contributors automatically. 

> This function works when the contributor has a public email on his/her profile page. If the contributor sets his/her email address private, then we can't send him an email.

![image](https://user-images.githubusercontent.com/45785633/228182641-835276f6-7aa9-48c0-a16b-3ef9cf452d30.png)

## Deploy PR Merge Notifier on your GitHub repo

### 0 Prerequisite 

1. You will need a [Sendgrid API key](https://app.sendgrid.com/settings/api_keys). If you do not already have one, [sign up here](https://app.sendgrid.com/settings/api_keys).
2. You will also need to sign into [flows.network](https://flows.network/) from your GitHub account. It is free.

### 1 Create from a template

[**Just click here**](https://flows.network/flow/createByTemplate/send-thank-you-email-to-contributor)

Click on the **Create and Build** button.


### 2 Configure the GitHub integration

Next, you will tell the bot which GitHub repo it needs to monitor for upcoming PRs.

* `github_owner`: GitHub org for the repo *you want to deploy the 🤖 on*.
* `github_repo` : GitHub repo *you want to deploy the 🤖 on*.

> Let's see an example. You would like to deploy the bot on `WasmEdge/wasmedge_hyper_demo` repo. Here `github_owner = WasmEdge` and `github_repo = wasmedge_hyper_demo`.

Click on the **Connect** or **+ Add new authentication** button to give the function access to the GitHub repo to deploy the 🤖. You'll be redirected to a new page where you must grant [flows.network](https://flows.network/) permission to the repo.

[<img width="450" alt="image" src="https://github.com/flows-network/github-pr-summary/assets/45785633/6cefff19-9eeb-4533-a20b-03c6a9c89473">](https://github.com/flows-network/github-pr-summary/assets/45785633/6cefff19-9eeb-4533-a20b-03c6a9c89473)

Close the tab and go back to the flow.network page once you are done. Click on **Deploy**.

### 3 Configure the SendGrid integration

Next, you will need to set up the email. Here we use SendGrid to do this.

* `sendgrid_sender_address`: the sender's email, which should be the same as your SendGrid setting.

<img width="500" alt="image" src="https://github.com/flows-network/pr-merge-notifier/assets/45785633/fc52db79-f735-42dd-8c27-9e319b752dbd">

Click on the **Connect** or **+ Add new authentication** button to give the function access to use your email address. You'll be redirected to a new page where you must grant [flows.network](https://flows.network/) permission to your SendGrid account.

  
<img width="500" alt="image" src="https://user-images.githubusercontent.com/45785633/227570457-94ad1092-e483-436c-be4e-624d1faff18a.png">

Close the tab and go back to the flow.network page once you are done. Click on **Deploy**.

## Wait for the magic

As soon as the flow function's status turns `ready` and the flow's status becomes `running`, the PR merge notifier goes live. Get connected with your contributor right away as contributors increase!

