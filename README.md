<h1 align="center"><code>status2signal</code></h1>
<p align="center">Status code to signal name converter</p>
<p align="center"><a href="https://github.com/NNBnh/status2signal/blob/main/LICENSE"><img src="https://img.shields.io/github/license/NNBnh/status2signal?labelColor=073551&color=4EAA25&style=for-the-badge" alt="License: GPL-3.0"></a> <img src="https://img.shields.io/badge/development-completed-%234EAA25.svg?labelColor=073551&style=for-the-badge&logoColor=FFFFFF" alt="Development completed"></p>
<p align="center"><a href="https://github.com/NNBnh/status2signal/watchers"><img src="https://img.shields.io/github/watchers/NNBnh/status2signal?labelColor=073551&color=4EAA25&style=flat-square"></a> <a href="https://github.com/NNBnh/status2signal/stargazers"><img src="https://img.shields.io/github/stars/NNBnh/status2signal?labelColor=073551&color=4EAA25&style=flat-square"></a> <a href="https://github.com/NNBnh/status2signal/network/members"><img src="https://img.shields.io/github/forks/NNBnh/status2signal?labelColor=073551&color=4EAA25&style=flat-square"></a> <a href="https://github.com/NNBnh/status2signal/issues"><img src="https://img.shields.io/github/issues/NNBnh/status2signal?labelColor=073551&color=4EAA25&style=flat-square"></a></p>

## 💡 About
`status2signal` is a tool to convert [status code](https://bash.cyberciti.biz/wiki/index.php?title=The_exit_status_of_a_command#Exit_Status) to [signal name](https://en.wikipedia.org/wiki/Signal_(IPC)#POSIX_signals) written in [`portable sh`](https://github.com/dylanaraps/pure-sh-bible) inspired by [Fish's `fish_status_to_signal` command](https://fishshell.com/docs/current/cmds/fish_status_to_signal.html).

## 🚀 Setup
### 🧾 Dependencies
- `sh` to process

### 📥 Installation
#### 🔧 Manually
- Option 1: using `curl`

```sh
curl https://raw.githubusercontent.com/NNBnh/status2signal/main/bin/status2signal > ~/.local/bin/status2signal
chmod +x ~/.local/bin/status2signal
```

- Option 2: using `git`

```sh
git clone https://github.com/NNBnh/status2signal.git ~/.local/share/status2signal
ln -s ~/.local/share/status2signal/bin/status2signal ~/.local/bin/status2signal
```

#### 📦 Package manager
For [`bpkg`](https://github.com/bpkg/bpkg) user:

```sh
bpkg install NNBnh/status2signal
```

For [Basher](https://github.com/bpkg/bpkg) user:

```sh
basher install NNBnh/status2signal
```

> *If you can and want to port status2signal to other package managers, feel free to do so.*

## ⌨️ Usage
Run 'status2signal' in the terminal:

```sh
status2signal STATUSCODES
```

## 💌 Credits
Special thanks to:
- [**Fish**](https://fishshell.com/docs/current/cmds/fish_status_to_signal.html) by [it's contributors](https://github.com/fish-shell/fish-shell/graphs/contributors)

<br><br><br><br>

---

> <h1 align="center">Made with ❤️ by <a href="https://github.com/NNBnh"><i>NNB</i></a></h1>
>
> <p align="center"><a href="https://www.buymeacoffee.com/nnbnh"><img src="https://img.shields.io/badge/buy_me_a_coffee%20-%23F7CA88.svg?logo=buy-me-a-coffee&logoColor=333333&style=for-the-badge" alt="Buy Me a Coffee"></p>
