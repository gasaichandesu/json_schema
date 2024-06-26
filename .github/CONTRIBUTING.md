# Contributing to json_schema

Looking to contribute something to the json_schema library? __Here's how you can help.__

+ __[Coding Standards](#coding-standards)__
  + [General Formatting Guidelines](#general-formatting-guidelines)
+ __[Using the Issue Tracker](#using-the-issue-tracker)__
  + [Reporting Bugs](#bug-reports)
  + [Feature Requests](#feature-requests)
  + [Submitting Pull Requests](#pull-requests)
+ __[Developer Workflow](#developer-workflow)__




## Coding standards

A lot can be gained by writing code in a consistent way.  Moreover, always remember that code is written and 
maintained by _people_. Ensure your code is descriptive, well commented, and approachable by others.

__ALWAYS__ adhere to the [Dart Style Guide].  _Please take the time to read it if you have never done so._

&nbsp;


### General formatting guidelines

+ __AVOID__ lines longer than 120 characters.
+ __AVOID__ using `dart format` as an excuse to ignore good judgement about
  whether your code is readable and approachable by others.

&nbsp;
&nbsp;



## Using the issue tracker

The issue tracker is the preferred channel for [bug reports](#bug-reports) and [feature requests](#feature-requests), 
but __please follow the guidelines:__

  + __Fill out the template we've provided.__

  + __Be Professional__
    + Please __do not__ derail or troll issues. Keep the discussion on topic and respect the opinions of others.

  + __Not that Professional__
    + Feel free to include _relevant_ animated gifs to drive home your message / request.

&nbsp;


### Bug reports

A bug is a _demonstrable problem_ that is caused by the code in the repository.

_Good bug reports are extremely helpful - thank you!__

__Guidelines for bug reports:__

1. __Search for existing issues.__ Duplicate issues can become cumbersome, and you'd help us out a lot by first 
   checking if someone else has reported the same issue. Moreover, the issue may have already been resolved with a 
   fix available.

2. __Record a screencast of yourself reproducing the issue__. 
  1. Be sure the problem exists in json_schema's code by building a 
     reduced test case that one of the reviewers can pull locally 
     and test out.

3. __Share as much information as possible.__ Include operating system and version, browser and version, etc. where appropriate. 

Always include steps to reproduce the bug.

__Example Bug Report:__

> Short and descriptive example bug report title
>
> A summary of the issue and the browser/OS environment in which it occurs. If
> suitable, include the steps required to reproduce the bug.
>
> 1. This is the first step
> 2. This is the second step
> 3. Further steps, etc.
>
> `<url>` - a link to branch with the reduced test case
>
> Any other information you want to share that is relevant to the issue being
> reported. This might include the lines of code that you have identified as
> causing the bug, and potential solutions (and your opinions on their
> merits).

&nbsp;


### Feature requests

Feature requests are welcome. But take a moment to find out whether your idea fits with the scope and aims of the 
project. It's up to *you* to make a strong case to convince the `json_schema` team of the merits of this feature. 
Please provide as much detail and context as possible.

&nbsp;


### Pull requests

Good pull requests - patches, improvements, new features - are a fantastic help. They should remain focused in scope 
and avoid containing unrelated commits.

__Please ask first__ before embarking on any significant pull request (e.g. implementing features, refactoring code, 
porting to a different language), otherwise you risk spending a lot of time working on something that the project's 
lead developers might not want to merge into the project.

Please adhere to the [Dart Style Guide] for all changes contained in your pull requests.

Adhering to the following process is the best way to get your work included in the project:

1. [Fork](http://help.github.com/fork-a-repo/) the project, clone your fork,
   and configure the remotes:

   ```bash
   # Navigate to the directory where you store repos locally
   cd ~/your-local-git-repo-spot
   # Clone your fork of the repo into the current directory
   git clone git@github.com:<your-username>/json_schema
   # Navigate to the newly cloned directory
   cd ~/your-local-git-repo-spot/json_schema
   # Assign the repo you forked from to a remote called "upstream"
   git remote add upstream git@github.com:Workiva/json_schema
   ```

2. If you cloned a while ago, get the latest changes from upstream:

   ```bash
   git checkout master
   git pull upstream master
   ```

3. Create a new topic branch that will contain your feature, change, or fix:

   ```bash
   git checkout -b <topic-branch-name>
   ```

4. Commit your changes in logical chunks. Please adhere to these 
   [git commit message guidelines](#git-commit-message-standards) or your code is unlikely be merged into the master 
   branch. Optionally, you can use Git's [interactive rebase](https://help.github.com/articles/interactive-rebase) 
   feature to tidy up your commits before making them public.

5. Write tests for your changes.  
  1. There are no exceptions.  
  2. If you're having trouble, reach out in your PR about how to best go about testing your changes.

6. If you have merge conflicts, locally merge the upstream master branch into your topic branch:

   ```bash
   git pull upstream master
   ```

7. Push your topic branch up to your fork:

   ```bash
   git push origin <topic-branch-name>
   ```

8. [Open a Pull Request](https://help.github.com/articles/using-pull-requests/)
    with a clear title and description - following all the [issue guidelines](#using-the-issue-tracker) listed above.

&nbsp;
&nbsp;


## Developer Workflow

The `json_schema` developer workflow couldn't be any more simple!

When you're ready to run the tests... run:

```bash
dart run dart_dev test
```


[Dart Style Guide]: https://www.dartlang.org/guides/language/effective-dart/style