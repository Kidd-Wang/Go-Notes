# Go-Notes
1. Install brew

Run the commands below:

!! Must use non-root account !!

>/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

>(echo; echo 'eval "$(/home/linuxbrew/.linuxbrew/bin/brew shellenv)"') >> /home/$USER/.bashrc

>eval "$(/home/linuxbrew/.linuxbrew/bin/brew shellenv)"

>brew -v

2. Install Go
> Go to https://go.dev/doc/install
> Download the latest tar file
> sudo tar -C /usr/local -xzf go1.22.0.linux-amd64.tar.gz
> Run 'vim ~/.bashrc' and add below
>    export PATH=$PATH:/usr/local/go/bin
>    export GOPATH=/var/www/go
>    export PATH=/opt/homebrew/bin/:$GOPATH/bin:$PATH
> Run 'source ~/.bashrc' to apply 
