# Data Transfer between machines using LAN.

Configure your both source and target machines using below process before initiating transfer.

If your system OS is windows 11 skip the windows 10 configuration

## **Configuration before initiating Transfer for windows 10:**

+Open Control panel
+Open “Network and internet”
+Open “Network and Sharing Centre”
+On left sidebar click on “Change Advanced sharing settings
+Under private section turn on “Network discovery” and “File and printer sharing”

![This is an image](https://raw.githubusercontent.com/thrinathreddynarahari/images/main/DTPicture1.png)

+Under Guest or Public Section turn on “Network discovery” and “File and printer sharing”

![This is an image](https://raw.githubusercontent.com/thrinathreddynarahari/images/main/DTPicture2.png)

+Under All Networks section turn on “Public folder sharing”, “Media Streaming”, “File sharing connections” and Turn OFF “Password protection sharing”.

![This is an image](https://raw.githubusercontent.com/thrinathreddynarahari/images/main/DTPicture3.png)

If your system os is windows 10 skip the windows 11 configuration and continue with "Making folders ready on Source Machine to transfer" section.

## **Configuration before initiating Transfer for windows 11:**

+Open Control panel
+Open “Network and internet”
+Open “Network and Sharing Centre”
+On left sidebar click on “Change Advanced sharing settings
+Make the changes as below image.

![This is an image](https://raw.githubusercontent.com/thrinathreddynarahari/images/main/DTPicture4.png)

***Restart Both Source and Target Machines after completing the above process.**

## **Making folders ready on Source Machine to transfer:**

+Select the folder you want to transfer right click on the folder and select “Properties.”

![This is an image](https://raw.githubusercontent.com/thrinathreddynarahari/images/main/DTPicture5.png)

+Select Sharing tab and click on share option.

![This is an image](https://raw.githubusercontent.com/thrinathreddynarahari/images/main/DTPicture6.png)

+Select option “Everyone”, click on “Add” and click on share.

![This is an image](https://raw.githubusercontent.com/thrinathreddynarahari/images/main/DTPicture7.png)

## **Modifying Target Machine to transfer:**

+Open network tab in file explorer and select the Source Machine

![This is an image](https://raw.githubusercontent.com/thrinathreddynarahari/images/main/DTPicture8.png)

+Copy and paste your files in your Machine.

## **To Transfer files faster follow the below procedure.**

+In Target machine run Command prompt as “Run as Administrator”

![This is an image](https://raw.githubusercontent.com/thrinathreddynarahari/images/main/DTPicture9.png)

+On the Target machine select the path of the folder you want to transfer.

![This is an image](https://raw.githubusercontent.com/thrinathreddynarahari/images/main/DTPicture10.png)

+Use the below command to transfer files

```
robocopy <SOURCE> <TARGET>
```

Example:

```
robocopy  "\\COGNINE-L101\copy-new" "D:\Newfield"
```

+User the below command to transfer files excluding node modules:

-Example:

```
robocopy  "\\COGNINE-L101\copy-new" "D:\Newfield" /mir /xd node_modules
```

## You can transfer multiple folders by opening multiple command prompts.
