The Python application that is being built by a team of six people is a Flask-based content management system.
The CI setup is as follows: for Python Pylint is a good choice for linting which ensures code quality and style guidelines. I would use pytest for some of the tests, then e2e testing could be done with Selenium or Cypress. If behavioral tests are needed, behave is good for this.

Git will be the version control system and GitHub Actions can be used for CI/CD tools.
Deciding between self-hosted or cloud-based CI environment can be a tricky choice but since it's a smaller team and they will not be working from the same location in-house nor is there such security concerns that warrant a closed-off system leads to cloud-based being the more convenient choice for this application's development cycle.
A self-hosted setup would provide more control over the infrastructure and security which can be crucial for more sensitive projects but since this is another CRUD-product, it's not worth the extra hassle and forcing everyone in the same location. Also the up-front cost of self-hosting and the maintenance can be more expensive for a smaller project compared to using easily scalable cloud solutions. Cloud-solutions would be more attractive for a team looking to focus on development rather than building infrastructure.

Alternatives to Jenkins or GitHub Actions include but aren't limited to GitLab CI, CircleCI and Travis CI and the team has to make an informed choice on which is the best option for them.
