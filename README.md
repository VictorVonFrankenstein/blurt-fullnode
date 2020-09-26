**Blurt Full Node Spec**

|  Component |  Size     |
|----------|-------------|
| **CPU** |  2+ Cores |
| **RAM** |    4GB   |
| **Storage** | 80+GB |

### Set up a Blurt Full Node

We've reduced setting up a full node to a single-line installer.  Run the following command as root on your fresh Debian 10 physical or virtual machine.  

```bash
bash <(curl -s https://raw.githubusercontent.com/ericet/blurt-fullnode/master/fullnode.bash)
```

Now you've just got to wait a bit for your machine to import 1.3 million Steem accounts and sync the Blurt Blockchain.  To monitor this process, do like:

```bash
journalctl -u blurtd -f
```
When you see individual blocks being produced, it's done and you're ready to proceed

Exit the scrolling monitoring logs with `Ctrl+C`

The script sets up a Blurt Full Node


