"Predicting customer feelings before they buy a product"

If you try executing the code along with the YouTuber, then at some point in time, you will get an error that "Daemon functionality is not supported on Windows". Therefore, to resolve this issue, you need to install WSL (Windows subsystem for Linux) and Ubuntu, on your Windows laptop/computer. To install WSL and Ubuntu, just run your command prompt as Administrator and run the below command:

wsl --install

This will take some time and then you will be asked to restart your computer/laptop. After the restart, open your Ubuntu terminal (remember, not WSL terminal) and give your first name in small letter case, and then give an easy password (Note: while entering, the password will not be visible). After that, a directory will be shown. Now, create a folder in Local disk D as "customer_satisfaction" and give that path in the Ubuntu terminal.

For example, the Linux path should be like this: cd /mnt/d/customer_satisfaction

Now, copy or download all the files and folders from my repository in the Local D > customer_satisfaction folder. Also, for the dataset, you can either download it from the YouTuber's GitHub or directly download it from the Google Drive link present in the data folder. (I can't upload the 50Mb dataset as the maximum dataset can be uploaded up to 25Mb)

Once you are in the customer_satisfaction directory, run the below Ubuntu commands, one by one.

sudo apt update

apt list --upgradable

sudo apt update

sudo apt install wget software-properties-common

sudo add-apt-repository ppa:deadsnakes/ppa

sudo apt update

sudo apt install python3.9

python3.9 --version

sudo apt install python3.9-distutils

wget https://bootstrap.pypa.io/get-pip.py

sudo python3.9 get-pip.py

python3.9 --version

pip install zenml

pip3 install zenml["server"]

pip uninstall zenml

pip install zenml["server"]

Now, when you run till here, from the above command, it will give you an error as Example: $PATH:/home/abdur/.local/bin. So, you need to copy it and paste in the below command and run it.

export PATH="$PATH:/home/abdur/.local/bin"

pip install zenml["server"] --no-warn-script-location

Now, you can start with the project.
You need to run the below commands.


