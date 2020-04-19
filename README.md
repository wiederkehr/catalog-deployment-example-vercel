# Publish Catalog on Zeit

Example for creating and publishing an instance of [Catalog](https://catalog.style/) using [Zeit](https://zeit.co/).

## 1. Install Catalog

1. Create a new Catalog following these [instructions](https://docs.catalog.style/installation/create-catalog).
2. Create a new repository on Github following these [instructions](https://help.github.com/en/github/creating-cloning-and-archiving-repositories/creating-a-new-repository).
3. Add your Catalog code to the new repository following these [instructions](https://help.github.com/en/github/importing-your-projects-to-github/adding-an-existing-project-to-github-using-the-command-line).

For more details about how to use Catalog, check out the [documentation](https://docs.catalog.style/).

## 2. Configure Zeit

1. Import a project on Zeit following these [instructions](https://zeit.co/docs/v2/git-integrations/zeit-now-for-github).
2. Leave the root directory field empty.
3. Add the script `yarn catalog-build` as the build command and `catalog/build` as the output directory.

![Zeit build settings](https://github.com/wiederkehr/catalog-deployment-example-zeit/raw/master/catalog/static/zeit-build-settings.png "Zeit build settings")

## 3. Publish to Zeit

- Everytime you push new code to the `master` branch, your Catalog will be deployed automatically.
- You can set up a custom domain for your site on Zeit.
