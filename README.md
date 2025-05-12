# Nexus Prover Node
You earn NEX Points by contributing compute and interacting with the Nexus ecosystem.

---

### Can I use multiple devices?
* Yes, you can connect as many devices as you want, including desktops, laptops, mobile phones, and servers
* You can link and manage all your devices from a single Nexus account.
* You can also prove computations in multiple browser tabs simultaneously.

---

## --> Create account
* Create an account at https://app.nexus.xyz.

* Follow the account linking instructions.

* Your contributions will earn NEX Points.

* Track your progress on the leaderboard.

* Manage all your nodes in one place.

---

## --> Contribute via Web browser
Login into the dashboard and press the button to start your node

https://app.nexus.xyz/

- You can run prover nodes on multiple browser tabs, desktops, laptops, mobile phones.
- Link and manage all your devices from a single Nexus account.
- More computations = More NEX points

---

## --> Contribute via Chromium (Browser on VPS)
You can install a Chromium browser on your Linux VPS and run a web-broswer based node on it too. [Guide to install Chromium on VPS](https://github.com/0xmoei/Install-Chromium-Linux-Browser)

* Open as many tabs as you want and run provers on all of them, LOL.
* I'm not sure about the performance but hey i'm just testing it.
* You'd better to have at least 1 CLI node near it too.

![image](https://github.com/user-attachments/assets/0e004e3c-f73e-4c32-bb86-0043b16259b7)

---

## --> Contribute via CLI
You might need a free +8GB RAM, you'd better to test it yourself since the testnet is under cunstructions
### 1. Install Dependecies
```bash
sudo apt update & sudo apt upgrade -y
sudo apt install screen curl libssl-dev pkg-config build-essential git-all protobuf-compiler -y
sudo apt update
```
```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
```bash
source $HOME/.cargo/env
```
```bash
rustup target add riscv32i-unknown-none-elf
```

### 2. Run Prover
**1- Start a screen to keep it running in the background**
```bash
screen -S nexus
```
**2- Install and run prover**
```bash
curl https://cli.nexus.xyz/ | sh
```

### 3. Link Node
1- After installation command completes, it asks you if you want to link your node press `2`
![image](https://github.com/user-attachments/assets/603d8a8e-5be5-485d-b4b8-76a9639aa836)

2- Enter you `node-id`
* To find your `node-id`, go  to https://app.nexus.xyz/nodes
* Click `Add Node`, click `Add CLI Node` and copy your `node-id` and paste in terminal

![image](https://github.com/user-attachments/assets/754e4b13-9400-4108-9c3f-b0bba6c40132)


### 4. Manage your Node screen:
* To minimze the screen: `CTRL+A+D`

* To return to screen: `screen -r nexus`

* To kill screen: `screen -XS nexus quit`

---


