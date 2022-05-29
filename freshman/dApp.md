# dApp

### Q1. Why am I getting Uncaught Error: Missing Provider?

This can be caused by a number of reasons, a common cause is running the html file without a hosted service. Metamask doesn't get injected except it's hosted. You can install and use lite-server or any other http server of your choice.

Check your url to know if it's hosted or not.
- Not hosted
<img width="1440" alt="dApp without lite-server" src="https://raw.githubusercontent.com/Jnrlouis/images/main/dApp1.png">
- Hosted
<img width="1440" alt="dApp with lite-server" src="https://raw.githubusercontent.com/Jnrlouis/images/main/dApp2.png">

### Q2. I have installed lite-server, Why am I still getting Uncaught Error: Missing Provider?

This can be caused by a number of reasons, if you have lite-server installed, make sure you're running it in the same directory as your index.html file. Also, Make sure your file is named index.html as lite-server only listens for files with that name.
