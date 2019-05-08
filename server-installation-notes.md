## GitHub Enterprise Server (GHES) installation notes

✅ | This course is fully compatible with any supported version* of GHES.
--- | ---

*Supported versions of GHES are visible by using the drop-down in the [official documentation](https://help.github.com/enterprise/).

### Course dependencies

The following are dependencies of the course. The course may continue to work without these dependencies, but learners won't experience the course as designed.

| Dependency                                                                                                               | Required? | Reason                                                                                                                                           | Alternative                                                                                                                                                                                    |
|--------------------------------------------------------------------------------------------------------------------------|-----------|--------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| GHES must be able to reach githubusercontent.com                                                                         | Yes       | Images used throughout the course are served from this domain. Learners will find broken images required to take the course without this access. | Manually download the images referenced in the `responses/` folder, upload them to an accessible domain, and replace the images in the `responses/` folder.                                    |
| Learner must be able to reach github.com and outside web                                                                 | No        | Links are provided to resources that live on the outside web.                                                                                    | Without access to resources on the outside web, learners will reach blocked resources. You can change the links to these resources in the `responses/` folder, and in the template repository. |
| [GitHub Pages](https://help.github.com/en/enterprise/2.16/admin/installation/configuring-github-pages-on-your-appliance) | No        | Used to teach the learner simple deployments from their own repo.                                                                                | Remove the step in `config.yml` that requires GitHub Pages is enabled. Look for references to GitHub Pages in the `responses/` folder and remove them.                                         |
