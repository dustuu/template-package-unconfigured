* [template-package-unconfigured](https://github.com/dustuu/template-package-unconfigured) shows what happens when the workflows are run with no configuration.
  * Without a `PACKAGE_NAME` variable, the `Build Release` workflow will skip both the `test` and `build` jobs:
  * ![image](https://github.com/vrchat-community/template-package/assets/101824882/d5f75f1a-6e72-4ea0-bcca-c3f1c7f69141)
  * The `Build Repo Listing` workflow will be trigged to run as well, but it will fail as expected because there are no published releases.
  * Both badges will be broken because there are no releases:
    * [![VPM Package Version](https://img.shields.io/vpm/v/com.vrchat.demo-template?repository_url=https%3A%2F%2Fdustuu.github.io%2Ftemplate-package-unconfigured%2Findex.json)](https://dustuu.github.io/template-package-unconfigured)
    * [![Code Coverage](https://dustuu.github.io/template-package-unconfigured/coverage/badge_linecoverage.svg)](https://dustuu.github.io/template-package-unconfigured/coverage)
