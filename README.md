# Ninja Bug

This branch is almost similar to the reported bug here: <https://developercommunity.visualstudio.com/t/-Build-single-file-failed-with-ninja:-er/10636057>

It is different to the mentioned bug (which uses this repo main branch to show the bug) in the following manner:

* Main CMakeLists.txt file is not in repo root folder, but in subfolder. The devenv.exe should be started in the subfolder `/src/targets/proj/subfolder`

To start devenv open folder via right-clicking the mentioned subfolder or use command line: `devenv.exe src/targets/proj/subfolder`
