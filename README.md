# git-branch-naming-convention
If you use git today, there are high chances that you're either using the famed git-flow or the more recent GitHub flow. 
Both these workflows depend extensively on using branches effectively — and naming a new branch is something many developers struggle with.

# Use issue tracker ID's in branch names
Most conventions recommend leading the branch name with prefixes like hotfix-, feature-, chore-, or some other variant of the categorization of tasks. Practically, if you are using an issue tracker, you’re tagging the category of the task in the issue tracker anyway — in addition to much more additional context. Using these categorical prefixes, this, seems redundant at least and requires additional decision-making when naming branches at worst. Leading with the issue tracker ID is convenient, requires minimal thinking, and has more advantages:

The issues created in the issue tracker, in most cases, are used for tracking the team’s progress. It becomes easy to correlate the relevant working branch with each task — especially when each developer is working on many issues at the same time.

Searching and filtering are much easier in the issue tracker. Once you know your issue number, it becomes easy to find the branch using autocomplete in the local git tree.

```
super-secret-project git:(master) git checkout 72<TAB>
2
722-add-billing-module  -- Apply suggestions from code review
3
720-submodules-rc       722-add-billing-module  723-fix-highlighting    728-fix-homepage-css
```


# Add a short descriptor of the task
While using the issue tracker ID itself is sufficient to identify a unique branch in a project in most cases, there could be chances that some more nuance is needed. For example, there could be multiple branches needed to work on one issue, possibly by different people.

Use a short, actionable descriptor of the task after the issue ID. This makes the branch name recognizable, distinct, and easy to search for in case you don’t have the issue ID handy. Make sure that the descriptor is concise, but descriptive enough to give you an idea of what’s going on in the branch.


# Use hyphens as seperators
This is a little opinionated, but hyphens make for good separators in branch names. You could use an underscore, _, too. The key is to be consistent, though.

And that’s it — just these three rules to keep in mind. No complex naming schemes or rules to follow make it easy for everyone in the team to stay on the same page. Naming things can be difficult at times, and it’s helpful to have simple heuristics. In a world where almost everyone is using some sort of issue tracking anyway, this approach makes git branch naming as easy as possible.

