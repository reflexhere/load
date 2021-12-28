## CHTA miner - Termux
Step 1. Download Termux from here: https://f-droid.org/en/packages/com.termux/

Step 2. Install Ubuntu 18.04 Bionic Beaver
        Type: pkg update -y && pkg install wget curl proot tar -y && wget https://raw.githubusercontent.com/AndronixApp/AndronixOrigin/master/Installer/Ubuntu/ubuntu.sh -O ubuntu.sh && chmod +x ubuntu.sh && bash ubuntu.sh
        Type: ./start-ubuntu.sh

## CHTA miner installation, follow all commands:
1. apt update
2. apt install wget ssh


## Get this file
   a. git clone https://github.com/reflexhere/load/blob/main/CHTATermux.tar.gz
  
   b. tar -xf CHTATermux.tar.gz   
   c. cd CHTATermux

3. uname -a (or uname -m : to determine whether your phone is 64bit or 32bit.
4. if your platform is arm32 type: chmod +x build_armhf.sh
5. if your platform is arm64 type: chmod +x bulid_arm64.sh
6. bash build_armhf.sh /  bash build_arm64.sh
7. cd armhf / arm64
8. cd cheetahcoin_v1.9.1.2_u16_armhf / cd cheetahcoin_v1.9.1.2_u16_arm64
9. ./cheetahcoind (create wallet folder & files)
10. nano cheetahcoin.conf 
11. use the arrow keys to navigate to modify your rpc username and password
12. CTRL+X+Y+ENTER to save file

##

13. cd ..
14. cp  -r cheetah_cpuminer  cheetah_cpuminer_chta
15. cd cheetah_cpuminer_chta
16. git pull
17. git checkout chta
18. nano cheetahcoin.conf
19. use the arrow keys to navigate to modify your rpc user>
20. CTRL+X+Y+ENTER to save file
21. cp cheetahcoin.conf  ~/.cheetahcoin/
    
         
## After complete syncing your CHTA wallet you can start mining
