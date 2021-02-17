# git commit message
### By Gontran Sion, the 2021-02-16.


### Git commit template

Configure Git to use your template file:
```
git config --global commit.template ~/.gitmessage
```
And save your git message file as : ~/.gitmessage

Refs:
![Pro Git](https://git-scm.com/book/en/v2)
![conventionalcommits](https://www.conventionalcommits.org/en/v1.0.0/)

.gitmessage file
```
#[type](optional scope): <subject>
#    Type
#        -> feat     - a new feature
#        -> fix      - a bug fix
#        -> docs     - changes in documentation
#        -> style    - everything related to styling
#        -> refactor - code changes that neither fixes a bug or adds a
#                      feature
#        -> perf     - special refactor, a code change that improves
#                      performance
#        -> test     - everything related to testing
#        -> chore    - updating build tasks, package manager configs...
#        -> revert   - Reverting things
#        -> build    - Build related changes
#        -> ci       - CI related changes
#    Scope
#        The scope provides additional contextual information
#        Is an optional part of the format
#        Allowed Scopes depends on the specific project
#        Don't use issue identifiers as scopes
#    Subject
#        "If applied, this commit will <your subject>"
#        The subject contains a succinct description of the change
#        Is a mandatory part of the format
#        Use the imperative, present tense: "change" not "changed"
#        nor "changes"
#        Don't capitalize the first letter
#        No dot (.) at the end
#
#(optional body)
#    The body should include the motivation for the change and contrast
#    this with previous behavior
#    Use the imperative, present tense: "change" not "changed" nor
#    "changes"
#    This is the place to mention issue identifiers and their relations
#
#(optional footer)
#    The footer should contain any information about breaking Changes
#    and is also the place to reference issues that this commit refers
#    to optionally reference an issue by its id
#    Breaking Changes should start with the word "BREAKING CHANGES:"
#    followed by space or two newlines
#    The rest of the commit message is then used for this
#
#Resolves: #123
#See also: #456, #789
```
