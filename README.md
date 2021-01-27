# New Server Installation Procedure

**1. Clean up**
 - first of all use **blower** to clean dust from main board , fans , slots and etc .
 - use dry electronic contact cleaner spray for cleaning cpu sockets , DIMM slots , PCIe slots and etc if it necessary .
 - * make sure all socket and slots are dry when you want to pluge the server power .

**2. Test**
 - remove cpus rams and all unnecessary carts and modules from the server .
 - drive server full of ram and cpu from test kit package. ( test kit pakage is a pack of rams and cpus that where tested before and we sure about their health )
 - turn the server on with default configuration. ( for example in hp servers you can use the **System maintenance switch** that desinged on mainboard for reseting or some other [features](https://techlibrary.hpe.com/docs/iss/DL380_Gen9/setup_install/GUID-83D6E12A-E5FB-4CDA-BBEB-2DB5559ED716.html) )
 - after server runs and passed post mode you can check server health in ilo / ipmi / iDrack etc .
 
**3. Naming and Inventory**
 - name the server " **H server number** " like **H120** , put a lable of server name somewhere behind the server chassis .
 - update chassis and all carts , modules , HDDs , items , etc that needs to put on this server in : **inventory --> devices --> target device --> inventory tab**
 
   sometimes you just have to assign some items in your target device .
 
**4. Assemble**
 - assemble collected items on the target server
 - * make sure that every modules are fit in their slots and heat sinks are agitated by silicone thermal grease.
 
**5. Update**
 - update firmwares , BIOS , IPMI , ILO and etc to latest stable version. ( for example in hp servers you should update SPP and IP with latest released version )
 
**6. Config and OS Installation**
 - set "saba" username by full access permission for ilo , ipmi , iDrack ..
 - set server name in ilo , ipmi , iDrack ..
 - for hp servers set ilo license in **ilo --> advance --> licensing**.
 - set ilo ip manualy by using IPAM allocated range and update server ilo interface ip in inventory. also set ip description.
 - set requested raid configuration in **Raid Controller** panel. 
 - install OS and set requested configuration.
 - set OS ip manualy by using IPAM allocated range and update server target interface ip in inventory. also set ip description.

**7. Rack Installation**
