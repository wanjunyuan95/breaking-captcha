# Github Best Practices

By: Hugh Wan (wanjunyuan@deakin.edu.au)

## Best practice for file naming

Files should be named consistently, short but descriptive. And also avoiding special characters or spaces in a file name. Instead of having periods, spaces or slashes, we highly recommend using capitals and underscores. Most importantly, the user should add a date and a version number so that it will be easier to track and review. Some of the elements to consider in a naming convention are:

- Date of creation
- Short descriptions
- Project name or number
- Analysis

Some examples for naming are:

- YYYYMMDD_Image_Modification
	- 20130420_tina_original.tiff
	- 20130420_tina_cropped.jpeg
	- 20130420_tina_mustache.jpeg

- LocationAnalysisVersion
	- CarnegieLakeWordCloudV1
	- CarnegieLakeMapV1
	- CarnegieLakeMapv2
	
Ideally, every member should have one folder by themselves so that the repository will not look as cluttered.

## Avoid commiting large files

In order to ensure reliable performance of the GitHub service, we limit the size of git objects that can be stored in GitHub. Currently the limit is set to 100MB, which means that only files 100MB and smaller can be committed to a git repository and pushed to GitHub. Attempting to push commits that contain files larger than 100MB will result in an error, and the commits will be rejected. 

While there is no fixed limit for the size of an individual repository, we enforce soft limits by warning users who are consuming an abnormally large amount of disk space. Binary files such as images, zip files, Word Documents, PDF files, etc, are better stored in an alternative storage location, such as AFS or Google Drive. 

## Make Effective use of Branching

Unlike other version control systems, creating branches in git is cheap and quick. Making effective use of branching allows you to very quickly work on a new feature or bug-fix and very easily compare the changes you’ve made to the main development branch, even across multiple commits. Utilizing branches also makes collaboration with others much easier, since everyone can work on a different branch and then merge changes in.

GitHub allows you to easily visualize merges in the web view via Pull Requests. In a Pull Request, you can see all the commits that will be merged, discuss the changes with your team, and view a summary of all pending changes. 

You can even protect certain branches in GitHub to prevent users from pushing directly to the branch. This workflow is great for large projects where changes need to be approved before they are merged into production.

## Write thoughtful Commit Messages

A well crafted commit message can be very useful when working on a project. The diff will tell you exactly what changed in a specific commit, but only the commit message will tell you why. One of the most important skills you can learn when learning git is how to write a good commit message.
