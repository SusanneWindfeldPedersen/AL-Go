# #10 Set up CI/CD for an existing per-tenant extension (BingMaps)
*Prerequisites: A GitHub account.
We will use the BingMaps sample app, which is on Azure DevOps here: https://dev.azure.com/businesscentralapps/_git/BingMaps
Copy following URL (a direct download of the main branch of the BingMaps sample) to the clipboard: https://dev.azure.com/businesscentralapps/BingMaps/_apis/git/repositories/BingMaps/items/items?path=/&versionDescriptor[versionOptions]=0&versionDescriptor[versionType]=0&versionDescriptor[version]=master&resolveLfs=true&$format=zip&api-version=5.0&download=true – you can download the .zip file and see the content of it.*

1. Navigate to https://github.com/microsoft/AL-Go-PTE and then choose **Use this template**.
![Use this template](/Scenarios/images/10a.png)
1. Enter **app2** as repository name and select **Create Repository from template**.
1. Under **Actions** select the **Add existing app or test app** workflow and choose **Run workflow**.
1. In the **Direct Download URL** field, paste in the direct download URL of the BingMaps sample from above.
1. When the workflow is complete, inspect the **Pull request**.
![Pull Request](/Scenarios/images/10b.png)
1. Merge the pull request. The **CI/CD** workflow will kick off.
![CI/CD](/Scenarios/images/10c.png)
1. After the workflow completes, you can investigate the output and see that everything works.
![Success](/Scenarios/images/10d.png)
1. Use [scenario 3](RegisterSandboxEnvironment.md), [scenario 4](CreateRelease.md), and [scenario 5](RegisterProductionEnvironment.md) to set up customer environments, publish and test the app.
---
[back](/README.md)
