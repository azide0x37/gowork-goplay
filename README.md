# gowork-goplay
Scripts for switching AWS credential environments. 

### Setup

 - duplicate ~/.aws/credentials twice to credentials.play and credentials.work
 - change default credential in each file
 - create following scripts
 - add below aliases to ~/.zshrc or ~/.bashrc or whatever.

####~/.awsPlay.sh
    '''shell
    cp -r ~/.aws/credentials.play ~/.aws/credentials
    '''

####~/.awsWork.sh
    '''shell
    cp -r ~/.aws/credentials.work ~/.aws/credentials
    '''

####~/.zshrc
    '''shell
    ...
    alias gowork="~/.awsWork.sh"
    alias goplay="~/.awsPlay.sh"
    ...
    '''
