## Using SSH on OSX

Mac OS X is shipped with the ssh client. You would not need to download a third party application to use ssh. The following instructions will help you get connected to the sunfire servers using the default ssh client included in Mac OS X.

Although you could install developer tools and run C code on your Mac machine, it is highly recommended that you write and test your C code using the sunfire server. There might be some difference in the compiler installed on your machine and the one on the sunfire server, and you getting used to the compiler error and warnings on the sunfire server would greatly help you when you do your practical exams (which would be conducted on the sunfire server)

1. Open the terminal application. You can either open Terminal app from the Applications folder, or simply search for Terminal using Spotlight.

2. You should notice that the terminal look and feels a bit like the sunfire. In fact, OSX and Solaris (the operating system behind sunfire) are UNIX systems, and hence they behave somewhat similarly under the hood. 

3. To connect to the sunfire server, type `ssh <SOC Username>@sunfire.comp.nus.edu.sg`, replacing <SOC Username> with your SOC Unix Account name. For instance, I would type `ssh soedar@sunfire.comp.nus.edu.sg`. A way to remember the command is `<username> [at] <the server you want to connect to>`

4. The first time you connect to the sunfire server, you should see a warning about the RSA key fingerprint. Make sure that the key is the same in the screenshot, and type yes.

5. You would then be prompted to enter your password. **NOTE:** the password field will *not* update even as you key in your password (i.e. the * characters will not appear as you type in your password). Enter your password and hit the enter key.

6. You should be able to see the Sunfire shell. Your sunfire files and settings should all be present now. Any command type in the terminal would now be executed on the sunfire server.

## Transfer files between Sunfire and OS X

### GUI Method

1. Download Cyberduck from [http://cyberduck.ch/](http://cyberduck.ch "Cyberduck")

2. If your machine is missing the Java runtime, you would be prompted to download the Java runtime. Install the Java runtime.

3. When you open CyberDuck, you should see the following interface. Tap on the + button at the bottom left.

4. The add new connection popup should appear. Fill in the fields as follow:
Type: SFTP (SSH File Transfer Protocol)
Nickname: <Anything you one. But preferably something like sunfire>
Server: sunfire.comp.nus.edu.sg
Username: <Your SOC UNIX Account Name>

5. The newly created connection should appear in the bookmark window. Double click on the one that you just created.

6. A login window should appear. Enter your password. Checking the Add to keychain box would save your password on your device, and you would not need to enter your password again.

7. The directory listing of the remote folder should appear. You can drag the files from the remote server to your local machine to download the file, or drag the files from your machine to the Cyberduck window to upload the files to the remote server.
