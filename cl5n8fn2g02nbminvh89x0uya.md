## Quick start of development work

### Node.js
We usually do not install node.js directly instead of managing it with NVM (Node Version Manager). NVM has a different implementation on different platforms. Windows' implementation is [here](https://github.com/coreybutler/nvm-windows), and Linux's one is [here](https://github.com/nvm-sh/nvm).

Take Windows as an example. After installing NVM, you can execute the command `nvm` to get all available usages. 

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1657932951283/YR8bzGUub.png align="left")

For Chinese users, you'd better set up the node mirror of Alibaba to speed up the node. 

```bash
nvm node_mirror https://npmmirror.com/mirrors/node
```

Then list all available node versions with the command `nvm list available`. We recommend installing LTS (Long Term Support) version.

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1657933360325/9kjC3QH8V.png align="left")

Then you can install what version you want. Execute the following commands.

```bash
nvm install 16  # Auto install the latest node.js, which's major version is 16
nvm use 16.16.0  # In my case, the newest version is 16.16.0
```

Validate your installation.

```bash
node -v
npm -v
```

### Common global NPM Packages

For Chinese users, the first step is to set up an NPM mirror of Alibaba.

```
npm config set registry http://registry.npmmirror.com
```

- [pnpm](https://pnpm.io)
```bash
npm install -g pnpm
pnpm -v
```

- [antfu/ni](https://github.com/antfu/ni)
```bash
npm i -g @antfu/ni
```

### JDK

View the article [Download Oracle JDK Without login](https://blog.edch.top/download-oracle-jdk-without-login) and install JDK and JRE in the specified directory such as `D:\dev-app\jdk\jdk1.8.0_333\` and `D:\dev-app\jdk\jre1.8.0_333`.

Create or update the system variable `JAVA_HOME` and set its value as `D:\dev-app\jdk\jdk1.8.0_333\` (The directory where you installed the JDK).

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1657935315747/emluonQsV.png align="left")

The add a record `%JAVA_HOME%\bin` in the system variable `path`.

Open a new terminal and check the Java version.

```bash
java -version
javac -version
javap -version
```

### Software Official Website

- [Git](https://gitforwindows.org)
- [Chrome](https://www.google.com/intl/zh-CN/chrome)
- [Jetbrains](https://www.jetbrains.com/toolbox-app)
- [MySQL Community Installer](https://dev.mysql.com/downloads/installer)
- [VS Code](https://code.visualstudio.com)




