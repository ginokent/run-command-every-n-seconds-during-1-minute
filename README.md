# run-command-every-n-seconds-during-1-minute

Run command every N seconds during 1 minute (for via cron)

## Installation

```bash
sudo bash -cx "curl -fLR https://raw.githubusercontent.com/djeeno/run-command-every-n-seconds-during-1-minute/master/bin/run-command-every-n-seconds-during-1-minute -o /usr/local/bin/run-command-every-n-seconds-during-1-minute && chmod +x /usr/local/bin/run-command-every-n-seconds-during-1-minute"
```



## How to use

If executing `TZ=UTC date` command every `5` seconds,  

```bash
run-command-every-n-seconds-during-1-minute 5 "TZ=UTC date"
```

For cron,  

```
* * * * * /usr/local/bin/run-command-every-n-seconds-during-1-minute 5 "TZ=UTC date" >>"$HOME/run-command-every-n-seconds-during-1-minute.log" 2>&1
```
