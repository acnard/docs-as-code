# docs-as-code
mkdocs deployment demo for documentation

The content is all stored under the doc folder of the repository. It consists of markdown files (.md extension) and images (typically screenshots) referenced by those markdown files, and can be organized into further subfolders. The convention adopted here is generally one folder per document, where each folder contains a single markdown file and all the images referenced by it.  

The content can be updated using a normal git worfklow, ie cloning the repo to a local machine and then editing the markdown files, or adding new ones, etc., and finally pushing the committed changes back to the origin. It is also possible to edit directly on github's web interface.

If a new markdown file is added, a link to it must be added in the **nav** section of the yml configuration file. Otherwise the file will not appear in the navigation sidebar of the deployed site.

After the source content is updated (changes committed and pushed to origin), the deployed site needs to be updated. This can be done with a mkdocs gh-deploy command on the local machine, or by launching the "build and deploy pages" action directly on github. 

you can view the deployment here: https://acnard.github.io/docs-as-code/
