# ncsu-guddati-research
This repository contains research materials related to computational mechanics and biomedical imaging developed under the NCSU Guddati research group.

# Accessing Repository Files in MATLAB

## Cloning the Repository Using Git

To clone the repository and access all files. This will create a local copy on your machine.

Steps to Clone:

1.	Open a terminal (or command prompt) on your computer.
2.	Navigate to the directory where you’d like to store the repository.
3.	Run the following command to clone the repository:

        git clone https://github.com/RPitsinger/ncsu-guddati-research.git
   
4.	After the repository has been cloned, open MATLAB and navigate to the directory where the repository is stored:

        cd('path-to-your-cloned-directory/ncsu-guddati-research');



## Fetching Specific Files Using GitHub API

If you only need to pull specific files from the repository (without cloning the entire repository), you can use MATLAB’s webread function to access individual files directly from GitHub.

Here’s an example of how to pull a raw file from the repository into MATLAB:

    url = 'https://raw.githubusercontent.com/RPitsinger/ncsu-guddati-research/main/path-to-file/yourfile.m';
    data = webread(url);

    % Now you can work with the 'data' in MATLAB
    disp(data);

Replace **path-to-file/yourfile.m** with the correct path to the file you wish to access.


## Pulling Latest Changes

If you have cloned the repository and want to fetch any updates that have been pushed to the GitHub repository, you can pull the latest changes directly from within MATLAB. Just open the command window in MATLAB and run:

    !git pull

This command ensures that your local copy is up-to-date with the GitHub repository.

## Working with MATLAB Git Integration

Alternatively, you can integrate Git with MATLAB to manage the repository directly within the MATLAB environment. To enable Git integration:

1.	Open MATLAB.
2.	Navigate to Home > Environment > Preferences > MATLAB > Git.
3.	Enable Use MATLAB’s Git integration.

You can now use Git commands directly from MATLAB to manage your local repository (clone, pull, commit, etc.).
