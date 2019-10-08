 # Git Templates
## Git Branch Naming 
The different types of branches we may use are:
* **Feature branches**
* **Bug branches**
* **Hotfix branches**

### Feature branches:
* naming convention: *feat/branch_name*
* used when developing a new feature or enhancement which has the potential of a development lifespan longer than a single deployment
* must adhere to static code check & peer-review (min 2 people)
* merged with no fast-forward

### Bug branches:
* naming convention: *bug/branch_name*
* used when there is a bug on the live site that should be fixed and merged into the next deployment
* must adhere to static code check & peer-review (min 2 people)
* deleted immediately after the merge
* should aim to deal with the root of the issue, not just one specific case (bug fix = system fix/improvement)

### Hotfix branches:
* naming convention: *hotfix/branch_name*
* used when it is needed to act immediately upon an undesired state of a live production version
* do not require static code check or peer-review (due to emergency)
* merged with no fast—forward
* hotfixes will be monitored and will require review to determine if this fixes root of the issue
* should be used extremely rarely


## Git Commit Naming Conventions
### Structure
      
      <type>(<scope>): <title>  
      <BLANK LINE>  
      <body>  
      <BLANK LINE>  
      <footer>

### Type tags
    - feature   (developing a new feature or system enhancement)
    - maintain  (refactoring, formatting, renaming..)
    - test      (writing or modifying tests)
    - bugfix   (fixing a case specific bug)


### Scope
    - anything specifying the place of the commit change  (example: validating-service)

### Title
      - a very short description of the change
      - imperative, present tense ("change" not "changed")
      - no capitalised first letter (optional)
      - no dot (.) at the end

### Body
      - should include the motivation for the change
      - may contain further explanations (when necessary)

### Footer
      - should contain any information like references to Jira issues related to this commit


## Authors
* **Jurica Kenda** - *Initial work* - [JuricaKenda](https://github.com/juricaKenda)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
