# VTEX-IO
Estudo do Ambiente Vtex.IO 

# Minimum Boilerplate Theme

The minimum Boilerplate Theme is basic store front model based on the VTEX IO Store Framework.

It should be used only when you want to start a new store theme without any pre-set configurations, as is the case with [Store Theme](https://github.com/vtex-apps/store-theme). 

While Store Theme gives developers a ready-to-go default store front structure, the Minimum Boilerplate Theme will enable you to build you store freely from scratch.

## Configuration

### Step 1 -  Basic setup

Access the VTEX IO [basic setup guide](https://vtex.io/docs/getting-started/build-stores-with-store-framework/2) and follow all the given steps. 

By the end of the setup, you should have the VTEX command line interface (Toolbelt) installed along with a developer workspace you can work in.

### Step 2 - Cloning the Minimum Boilerplate Theme repository

[Clone](https://help.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository) this repository to your local files to be able to effectively start working on it.

Then, access the repository's directory using your terminal. 

### Step 3 - Editing the `Manifest.json`

Once in the repository directory, it is time to edit the Minimum Boilerplate `manifest.json` file. 

Once in are in the file, you must replace the `vendor` and `account` values. `vendor` is the account name you are working on and `account` is anything you want to name your theme. For example:

```json
{
  "vendor": "storecomponents",
  "name": "my-test-theme",
}
```

### Step 4 -  Installing required apps

In order to use Store Framework and work on your store theme, it is needed to have both `vtex.store-sitemap` and `vtex.store` installed.

Run  `vtex list`  and check whether those apps are already installed. 

If they aren't, run the following command to install them: `vtex install vtex.store-sitemap vtex.store -f`

### Step 5 -  Uninstalling any existing theme

By running `vtex list`,  you can verify if any theme is installed.

It is common to already have a `vtex.store-theme`  installed when you start the store's front development process. 

Therefore, if you find it in the app's list, copy its name and use it together with the command `vtex uninstall`. For example:

```json
vtex uninstall vtex.store-theme
```

### Step 6- Run and preview your store

Then time has come to upload all the changes you made in your local files to the platform. For that, use the `vtex link` command. 

If the process runs without any errors, the following message will be displayed: `App linked successfully`. Then, run the `vtex browse` command to open a browser window having your linked store in it.

This will enable you to see the applied changes in real time, through the account and workspace in which you are working.

## MY WORKSPACE -> workspacerodolfodev


### GLOSSARY

##### Query schema -> A query schema é uma das [props do search result custom query](https://developers.vtex.com/vtex-developer-docs/docs/vtex-search-result) com ela é possível controlar a busca que a nossa landing page deverá fazer. Para saber todas as possibilidades da query schema, [veja sua documentação aqui.](https://developers.vtex.com/vtex-developer-docs/docs/vtex-search-result#step-3---defining-how-the-search-query-data-should-be-fetched)


### CHECK LIST -  VTEX.IO COURSE
[x] - [Blocos básicos](https://learn.vtex.com/docs/course-basic-blocks-lang-pt);
[x] - [Layouts complexos](https://learn.vtex.com/docs/course-layout-blocks-lang-pt)
[x] - [Tornando sua loja única](https://learn.vtex.com/docs/course-styles-course-lang-pt)
[x] - [Site Editor e conteúdo](https://learn.vtex.com/docs/course-content-workflow-lang-pt)
[x] - [Melhorando performance](https://learn.vtex.com/docs/course-store-performance-lang-pt)
[] - [Blocos customizados](https://learn.vtex.com/docs/course-store-block-lang-pt)
[] - [Serviços](https://learn.vtex.com/docs/course-service-course-lang-pt)
[] - [Aplicações administrativas](https://learn.vtex.com/docs/course-admin-lang-pt)
[] - [Chamando as APIs de Commerce](https://learn.vtex.com/docs/course-calling-commerce-apis-lang-pt)