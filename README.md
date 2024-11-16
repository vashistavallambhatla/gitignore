Observations:

-> The closer the .gitignore file is to the actual file, the higher the precedence, if the root .gitignore ignores all the .log files (*.log) and the closest .gitignore asks .log files not to be ignore (!*.log), the perecedence will be given to the latter .gitignore

-> the files mentioned in .gitignore are not being tracked, meaning the changes made to that file aren't showing up in git status 

-> If a file is already being tracked by Git, adding it to .gitignore will not stop Git from tracking it. I had to use 'git rm --cached <file_name>' to stop the tracking.

-> The files ignored were not pushed to this repo either as expected.
