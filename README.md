![Logo](https://github.com/Sushantdbg/reviveMyUSB/blob/main/Assets/Logo.png?raw=true)

[![MIT License](https://img.shields.io/apm/l/atomic-design-ui.svg?)](https://github.com/tterb/atomic-design-ui/blob/master/LICENSEs)


## FAQ

#### What is this about?

There are situations where one after doing a Linux installation session isn't able to use  flash drive on their native Windows PC, so this guide/project is all about guiding the steps to make the USB flash drive back to life

#### Are there any pre-requisites?

Nothing special just a windows machine and your flash drive.

## Tech Stack

**Windows Command Line**

## Procedure
I will adding the corresponding screenshot as per my PC which may or maynot be same for your pc for example the disk number of flash drive.

All such factors are addressed as well as will be handled with the corresponding details of steps

#### THIS PROJECT/INSTRUCTIONS IS/ARE PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND

### Instructions starts here

Step 1: Start CMD with admin privilege

Step 2:
```bash
diskpart
```
Step 3:
```bash
list disk
```
Step 4:
```bash
select disk <disk number of flash drive>
```
Step 5:
```bash
list disk
```
Step 6:
```bash
clean
```
Step 7:
```bash
convert gpt
```
Step 8:
```bash
clean
```
Step 9:
```bash
list disk
```
Step 10:
```bash
create partition primary
```
Step 11:
```bash
list partition
```
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

- [@Sushantdbg](https://github.com/Sushantdbg)
- [@Pallavikumarimdb](https://github.com/Pallavikumarimdb)
