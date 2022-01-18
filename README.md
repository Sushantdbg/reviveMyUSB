![Logo](https://github.com/Sushantdbg/reviveMyUSB/blob/main/Assets/Logo.png?raw=true)

[![MIT License](https://img.shields.io/apm/l/atomic-design-ui.svg?)](https://github.com/tterb/atomic-design-ui/blob/master/LICENSEs)

#
## FAQ
### What is this about?

There are situations where one after doing a Linux installation session isn't able to use  flash drive on their native Windows PC. When one tries to format it using the native windows GUI formatting they might face error like "DIRECTORY DOESN'T EXIST" or furthermore when trying to use the Disk Management Utility errors like below pops up... 

![Error that you might be getting while trying to format](https://github.com/Sushantdbg/reviveMyUSB/blob/main/screenshots/00.png?raw=true)

...so this guide/project is all about guiding the steps to make the USB flash drive back to life

### Are there any pre-requisites?

Nothing special just a windows machine and your flash drive.
#

## Tech Stack

**Windows Command Line**
#

## Procedure
I will adding the corresponding screenshot as per my PC which may or maynot be same for your pc for example the disk number of flash drive.

All such factors are addressed as well as will be handled with the corresponding details of steps

#### BEFORE GOING AHEAD CONSIDER THE FACT THAT THIS PROJECT/INSTRUCTIONS IS/ARE PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND

### Instructions starts here

Step 1: Start CMD with admin privilege

![Starting with admin privilege](https://github.com/Sushantdbg/reviveMyUSB/blob/main/screenshots/01.png?raw=true)

Step 2:
```bash
diskpart
```
![img02](https://github.com/Sushantdbg/reviveMyUSB/blob/main/screenshots/02.png?raw=true)


Step 3:
```bash
list disk
```
![img02](https://github.com/Sushantdbg/reviveMyUSB/blob/main/screenshots/03.png?raw=true)


Step 4:
```bash
select disk <disk number of flash drive>
```


![img02](https://github.com/Sushantdbg/reviveMyUSB/blob/main/screenshots/04.png?raw=true)


Step 5:
```bash
list disk
```


![img02](https://github.com/Sushantdbg/reviveMyUSB/blob/main/screenshots/05.png?raw=true)


Step 6:
```bash
clean
```


![img02](https://github.com/Sushantdbg/reviveMyUSB/blob/main/screenshots/06.png?raw=true)


Step 7:
```bash
convert gpt
```


![img02](https://github.com/Sushantdbg/reviveMyUSB/blob/main/screenshots/07.png?raw=true)


Step 8:
```bash
clean
```


![img02](https://github.com/Sushantdbg/reviveMyUSB/blob/main/screenshots/08.png?raw=true)


Step 9:
```bash
list disk
```


![img02](https://github.com/Sushantdbg/reviveMyUSB/blob/main/screenshots/09.png?raw=true)


Step 10:
```bash
create partition primary
```


![img02](https://github.com/Sushantdbg/reviveMyUSB/blob/main/screenshots/10.png?raw=true)


Step 11:
```bash
list partition
```


![img02](https://github.com/Sushantdbg/reviveMyUSB/blob/main/screenshots/11.png?raw=true)


Step 12:
```bash
select partition <number according to one's personal flash drive>
```
Step 13:
```bash
active
```
Step 14:
```bash
format fs=fat32 quick
```
Step 15:
```bash
exit
```
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

#### 1. Fork the Project
#### 2. Create your Feature Branch
#### 3. Commit your Changes
#### 4. Push to the Branch
#### 5. Open a Pull Request

## Contributors

- [Sushant Kumar](https://github.com/Sushantdbg)
- [Pallavi Kumari](https://github.com/Pallavikumarimdb)
