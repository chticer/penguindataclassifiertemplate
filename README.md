# Penguins Data Classifier

This is a template repository of using the Flask framework in Python to predict what kind of penguin that a trained machine learning model thinks it would be classified under with specified feature values.

**Classifier Features**

- Culmen length (in millimeters)
- Culmen depth (in millimeters)
- Flipper length (in millimeters)
- Body mass (in grams)

**Classifier Label**

The species of the penguin.

Possible labels:

- Adelie
- Chinstrap
- Gentoo

## Instructions

The `app.py`, `index.html`, and `predict.html` files contain starter code with key features missing. Information on what code is missing is provided in comments.

**GitHub**

Login to GitHub and create an empty GitHub repository.

**Terminal**

Open a terminal window and navigate to your desired path.

1. Set Git credentials

Replace **github-username** and **github-email-address** with your GitHub's username and email address, respectively.

```
git config --global user.name "github-username"
git config --global user.email "github-email-address"
```

2. Clone the repository

```
git clone https://github.com/chticer/penguindataclassifiertemplate
```

```
cd penguindataclassifiertemplate
```

3. Update remote repository location

Replace **github-repository-url** with the GitHub repository URL that was created.

```
git remote set-url origin github-repository-url.git
```

**Visual Studio Code**

Open the cloned repository (File > Open Folder).

Add any Azure Machine Learning workspace models created with this dataset into the `models` folder. One model is included.

Run the Flask application (open `app.py` then Run > Run Without Debugging).

Stage, commit, and push files using Source Control on the left side.

**Azure App Service Deployment**

Create an Azure app service.

1. Go to https://portal.azure.com/ and search for the "App services" resource.
1. Click Create > Web App. Fill in the following fields then click Review + create:
    - **Subscription**: Select your Azure subscription.
    - **Resource Group**: Select an existing one or create a new one.
    - **Name**: Enter an unique website name.
    - **Runtime stack**: Select a Python version.
    - **Region**: Select the closest region.
    - **Linux Plan**: Create a new app service plan.
    - **Pricing plan**: Select a plan based on your needs.
1. Once the resource has been deployed, go to the resource.
1. On the left side, click Deployment > Deployment Center.
1. Click the Settings tab. Fill in the following fields then click Save:
    - **Source**: GitHub (authorize your GitHub account with Microsoft Azure App Services if necessary)
    - **Organization**: Select your GitHub username.
    - **Repository**: Select the GitHub repository.
    - **Branch**: Select the origin branch of the GitHub repository.
1. View the website. To find the website URL, on the left side, click Overview. The website URL will be shown next to Default domain.

## Special Thanks

This repository is part of an Azure Machine Learning workshop conducted with students, which was made possible by a grant from the Department of Homeland Security, at The University of Texas Rio Grande Valley on Saturday, August 12, 2023.

**Workshop Leaders**
- [@alfazick](https://github.com/alfazick) (Dr. Askar Nurbekov)
- [@chticer](https://github.com/chticer) (Mr. Charlie Ticer)
- [@emmett-tomai](https://github.com/emmett-tomai) (Dr. Emmett Tomai)

We would also like to thank the students for their participation and the IT and department administrative staff and student workers for their help, time, and resources in this workshop.

The penguins dataset used for training models were provided by Palmer Archipelago (Antarctica).

> Gorman KB, Williams TD, Fraser WR (2014) Ecological Sexual Dimorphism and Environmental Variability within a Community of Antarctic Penguins (Genus Pygoscelis). PLoS ONE 9(3): e90081. doi:10.1371/journal.pone.0090081

See this [README](https://github.com/dickoa/penguins/blob/master/README.md) for additional attributions.
