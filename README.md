# ASEN4018_Green
This repository houses all software for a Small Space Debris Detection and Tracking Satellite for the CU Boulder ASEN 4018 Senior Projects 2026-27 class, specifically the Green Team. 

# 0. Table of Contents
TODO

# 1. Getting Started
> If you don't know much about Git/GitHub and would like to learn, there are a bunch of resources online, but I also made a repository which can sorta serve as a reference/starting point for a lot of the important workflow. If that sounds like it might be useful, you can access it at [https://github.com/bassett-luke/GitHub-Reference](https://github.com/bassett-luke/GitHub-Reference), let me know if y'all have any problems with any of the commands/instructions. -Luke

## 1.1 Cloning the Repository to Your Local Machine
If you want just the flight software repository (e.g. deployment on flight computer), go to [https://github.com/bassett-luke/asen4018-green-fsw](https://github.com/bassett-luke/asen4018-green-fsw), and follow the cloning instructions there (TODO). 

Since we're using Git Submodules (section about that not included in the reference (yet)), we have a little bit different workflow for pulling the files down than a standard `git clone`. 

If you're looking to just work on analysis or ground data processing, and you don't need to work on the flight software at all, you can clone just this repository like normal:

```shell
git clone https://github.com/bassett-luke/ASEN4018_Green
```

To pull down the FULL software stack (this master repository plus the flight software repository), run the following: 

```shell
git clone --recurse-submodules https://github.com/bassett-luke/ASEN4018_Green
```

If you pulled down just this repository without the flight software, you should already have an empty **asen4018-green-fsw** repo, so you just need to run the following to pull in the flight software:

```shell
git submodule update --init --recursive
```

## 1.2 Workflow
> Message me on Teams and I can give you commit access to either or both repositories! -Luke
