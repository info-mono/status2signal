<h1 align="center"><code>status2signal</code></h1>
<p align="center">Status code to signal name translate</p>
<p align="center"><a href="https://github.com/info-mono/status2signal/blob/main/LICENSE"><img src="https://img.shields.io/github/license/info-mono/status2signal?labelColor=383838&color=585858&style=for-the-badge" alt="License: GPL-3.0"></a> <a href="https://gist.github.com/NNBnh/9ef453aba3efce26046e0d3119dab5a7#development-completed"><img src="https://img.shields.io/badge/development-completed-%23585858.svg?labelColor=383838&style=for-the-badge&logoColor=FFFFFF" alt="Development completed"></a></p>

## 💡 About
`status2signal` is a tool to translate [status code](https://bash.cyberciti.biz/wiki/index.php?title=The_exit_status_of_a_command#Exit_Status) to [signal name](https://en.wikipedia.org/wiki/Signal_(IPC)#POSIX_signals) written in [`portable sh`](https://github.com/dylanaraps/pure-sh-bible) inspired by [Fish's `fish_status_to_signal` command](https://fishshell.com/docs/current/cmds/fish_status_to_signal.html) and [Starship's Status module](https://starship.rs/config/#status).

## 🚀 Setup
### 🧾 Dependencies
- [Unix commands](https://en.wikipedia.org/wiki/List_of_Unix_commands) to process

### 📥 Installation
#### 🔧 Manually
Option 1: using `curl`
```sh
curl https://raw.githubusercontent.com/info-mono/status2signal/main/bin/status2signal > ~/.local/bin/status2signal
chmod +x ~/.local/bin/status2signal
```

Option 2: using `git`
```sh
git clone https://github.com/info-mono/status2signal.git ~/.local/share/status2signal
ln -s ~/.local/share/status2signal/bin/status2signal ~/.local/bin/status2signal
```

#### 📦 Package manager
For [Bpkg](https://github.com/bpkg/bpkg) user:
```sh
bpkg install info-mono/status2signal
```

For [Basher](https://github.com/basherpm/basher) user:
```sh
basher install info-mono/status2signal
```

> *If you can and want to port status2signal to other package managers, feel free to do so.*

## ⌨️ Usage
Run 'status2signal' in the terminal:
```sh
status2signal STATUSCODES
```

Here is the list of statuses and signals that they will be translated to:
|Status|Signal     |
|------|-----------|
|`0`   |empty      |
|`1`   |`ERROR`    |
|`2`   |`USAGE`    |
|      |           |
|`126` |`NOPERM`   |
|`127` |`NOTFOUND` |
|      |           |
|`129` |`SIGHUP`   |
|`130` |`SIGINT`   |
|`131` |`SIGQUIT`  |
|`132` |`SIGILL`   |
|`133` |`SIGTRAP`  |
|`134` |`SIGABRT`  |
|`135` |`SIGBUS`   |
|`136` |`SIGFPE`   |
|`137` |`SIGKILL`  |
|`138` |`SIGUSR1`  |
|`139` |`SIGSEGV`  |
|`140` |`SIGUSR2`  |
|`141` |`SIGPIPE`  |
|`142` |`SIGALRM`  |
|`143` |`SIGTERM`  |
|`144` |`SIGSTKFLT`|
|`145` |`SIGCHLD`  |
|`146` |`SIGCONT`  |
|`147` |`SIGSTOP`  |
|`148` |`SIGTSTP`  |
|`149` |`SIGTTIN`  |
|`150` |`SIGTTOU`  |
|`151` |`SIGURG`   |
|`152` |`SIGXCPU`  |
|`153` |`SIGXFSZ`  |
|`154` |`SIGVTALRM`|
|`155` |`SIGPROF`  |
|`156` |`SIGWINCH` |
|`157` |`SIGIO`    |
|`158` |`SIGPWR`   |
|`159` |`SIGSYS`   |

> *Other positive integer will be translated to `ERROR`*.

## 💌 Credits
Special thanks to:
- [**Fish**](https://fishshell.com/docs/current/cmds/fish_status_to_signal.html) by [it's contributors](https://github.com/fish-shell/fish-shell/graphs/contributors)
- [**Starship**](https://starship.rs) by [it's contributors](https://github.com/starship/starship/graphs/contributors)

<br><br><br><br>

---

> <h1 align="center">Made with ❤️ by <a href="https://github.com/info-mono"><code>@info-mono</code></a></h1>
>
> <p align="center"><a href="https://www.buymeacoffee.com/nnbnh"><img src="https://img.shields.io/badge/buy_me_a_coffee%20-%23F7CA88.svg?logo=buy-me-a-coffee&logoColor=333333&style=for-the-badge" alt="Buy Me a Coffee"></a></p>
