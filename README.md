# A Testing Repo for GitHub Pages

A basic splash page for testing out the GitHub Pages feature (free hosting).

> This page is available to view at  
> [https://codeadamca.github.io/github-pages-deploy-html/](https://codeadamca.github.io/github-pages-deploy-html/)  

## Deploy a Static Page to GitHub Pages

[GitHib Pages] allows you to deploy your static HTML, JavaScript, and CSS pages to a GitHub or custom domain. To deploy a repository follow these steps:

1. Create a new standard repository, let's assume it's named `github-pages`: 

    ![New Repository](_readme/screenshot-new-repo.png)

    - Give the repo the name `github-pages-deploy-html`
    - Give the repo a brief description `Deploying a static page using GitHub Pages.`
    - For the rest, just leave the defaults
    - Click `Create repository`

2. Using the terminal clone the repo:

    ```
    git clone https://github.com/codeadamca/github-pages-deploy-html
    ```

3. Open the new `github-pages-deploy-html` folder using your IDE of choice. I use Visual Studio Code. Add an `index.html` and add some basic HTML content:

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>GitHub Pages</title>
    </head>
    <body>
        <h1>Hello GitHub Pages!!</h1>
    </body>
    </html>
    ```

4. Push the changes to your GitHub repo:

    ```
    git add .
    fit commit -m "Added home page"
    git push origin main
    ```

5. Using the browser, navigate back to `githib-pages-deploy-html` repo, click on the `settings` tab, and then `Pages`.

6. Choose `Deploy from branch`, the branch name and folder you want to deploy, then click save:

    ![GitHub Pages](_readme/screenshot-pages.png)

7. Wait for a minute or two and then the GitHub URL will be functional. The URL will be:

    ```
    http://<REPO_NAME>.<GITHUB_USERNAME>.ca/
    ```

## Custom Domain

You can use a custom domain (or subdomain) you have registered from a domain name provider. 

Go back to the repo settings and choose `Pages`. Enter the custom domain, choose whether or not to `Enforce HTTPS`, and click `Save`:

![Custom Domain](_readme/screenshot-custom.png)

Log in to your domain name provider and navigate to your domain name DNS settings. Add four A records pointing the domain to GitHub:

```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

In my domain name provider the settings looks like this:

![DNS Settings](_readme/screenshot-dns.png)

For more information on setting up your custom doamin checkout the [GitHub Documentation](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site).

***

## Repo Resources

* [GitHib Pages](https://pages.github.com/)
* [GitHub - Custom Domain Documentation](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site)

<br>
<a href="https://codeadam.ca">
<img src="https://cdn.codeadam.ca/images@1.0.0/codeadam-logo-coloured-horizontal.png" width="200">
</a>
