page_title: Source control integrations
page_description: How to watch images using Shippable's Lighthouse Feature
page_keywords: lighthouse, shippable ci, documentation, shippable, watch docker images

# Source Control Management systems

Integrations for GitHub and Bitbucket do not need to be set up manually on Shippable. These are automatically configured for you when you sign in with your credentials for these services, or when you add them in the `Git identity` section of Account Settings. 

## GitHub
In order to integrate with your GitHub account, we automatically set up an Account integration when you log in using your GitHub credentials. You do not have to do anything to set this up further.

## Bitbucket
In order to integrate with your Bitbucket account, we automatically set up an Account integration when you log in using your Bitbucket credentials. You do not have to do anything to set this up further.

## GitHub Enterprise
We do not support signing in to Shippable directly with your GitHub Enterprise credentials. In order to use Shippable for your GitHub Enterprise repositories, you will need to sign in with GitHub or Bitbucket and then add an account integration as follows :

- Click on the gear icon for Account Settings in the top navigation bar. Select the `Integrations` tab.
- Click on `Add Integration` and from the dropdown for **Integration type**, select `GitHub Enterprise`
- Enter a name for this integration in the **Integration name** textbox.
- Enter the URL for your GitHub Enterprise instance. The URL should be in the format https://(git hub enterprise URL)/api/v3
- You will need to add a token from your GitHub Enterprise account with the right permissions. To do this -
    - Go to your GitHub Enterprise account settings and in the left menu, select 
   `Personal access tokens`.
    - Click on `Generate token` and on the Generate Token page, select the following permissions.
    - Click on `Generate token`, and copy the generated token immediately. This is important since you will not see the token once you navigate away from this page.
    - Paste the token in your Integration on Shippable and click on `Save`.   
- After adding a GitHub Enterprise integration, you should go to the Account Settings tab and `Sync` your account.
- Go to your Shippable dashboard and check to make sure you have your GitHub Enterprise subscriptions in the CI dropdown.

You can now enable projects, run CI, etc just like with GitHub or Bitbucket subscriptions.