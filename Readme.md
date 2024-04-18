
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

### Merge conflict
Now let's say after release1 is updated, the group starts go on working and one guy updates the feature1 file in the feature1 branch.
However, another guy also update the feature1 file but in the release1 branch.
And now one two branches are going to be merged, there will be a conflict happens.

![git_conflict_example](/image/git_conflict_example.png)

If the console gives these notice, it means the merge has failed. 
The files happening conflict will be added with the conflict message and be removed from the current git files.
![git_conflict_file](</image/git_conflict_file.png>)

After fixed the conflict in the file with any kinds of ways, running the git add command to add the file back in the git system.
```shell
git add [conflict_file_name]
```
And then, the conflict of the merge is solved.
In conclusion, when the merge conflict is happening, the file need to be add again as a sign telling git conflict has been solved.


