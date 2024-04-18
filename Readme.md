
This project is sample for learning git commands.

## Git merge command

```shell
git merge [branch]
```
This command is used to merge the content in one branch into the current branch.

### Merge example
There are two branches here each with a "feature" file in it, which are feature1 and feature2.
In the scenario made right here, the project includes two different feature functions which are feature1 and feature2.
The final release eddition should contain both feature1 and feature2, and it can be achieved by using the merge command.

```shell
git switch -c release1
git merge feature1
git merge feature2
```
After using these commands we will have a new branch with both features implemented.

![git_merge_example](/image/git_merge_example.png)
