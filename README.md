# Scanners

A collection of network scanners designed to check websites that are exposed to amplification attacks.
I take no responsibility on how you are using this program.
It was designed and should be used for pentesting with consent from the website's owner.


## Installation Instrunctions

```
sudo apt update
sudo apt install git
git clone https://github.com/yTax/scanners.git
cd scanners
chmod +x *
./(choose a scanner you want to use)
```

## Usage

Note: I choose the ts3scanner as an example this applies to any of the scanners except DNS, if you're confused you can just run it and it will tell you how to use it.

This is how you would run any of them except for DNS
```
./ts3scan [STARING IP] [END IP] [OUTPUT.txt] [Threads] [Delay in MS]
```

And this is how you would use the DNS scanner
```
./dnsscan [Starting class] [Ending class] [Output.txt] [Threads] [Delay in MS]
```
A usage example would be the following:

For any of them except DNS (Again snmp was choosen has an example)
```
./snmpscan 10.0.0.0 100.255.255.255 ssdp.txt 100 5
```

For the DNS scanner
```
./dnsscan 1 2 dns.txt 200 100
```
## Thanks to

Thanks to Xavier, a friend of mine who let me use his snmpscan
