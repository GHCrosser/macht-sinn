# macht-sinn

Ergibt das Sinn?

## Description

This script generates a Blacklist for ad- and malwareblocking. Remove those ads **without altering your browser-fingerprint**, see the web **as you like**. Let it work on your Router for an adblocking-monster fixing the **whole network** behind it. Ever seen an **ad-free Smartphone**?

Since this script needs write-access to the hostfile defined in $ADNAME, it will most likely need root-privileges (sudo).

## Installation

0. Change into the target Git directory
0. Execute 'git clone https://github.com/GHCrosser/macht-sinn.git'
0. Read 'machtsinn.conf' carefully!
0. Edit 'machtsinn.conf' to your needs
0. Edit 'CONF' in machtsinn.sh to '/etc/machtsinn/machtsinn.conf' if i forgot it
0. Place files to the intended destinations
0. Fetch the blocklist with 'sudo machtsinn.sh -g'
0. Enjoy an almost ad-free Internet

## Fetched Blocklists (default)

0. http://pgl.yoyo.org/adservers/serverlist.php?hostformat=hosts&mimetype=plaintext
0. http://someonewhocares.org/hosts/hosts
0. http://www.malwaredomainlist.com/hostslist/hosts.txt
0. http://winhelp2002.mvps.org/hosts.txt
0. http://hosts-file.net/download/hosts.txt
0. http://hosts-file.net/hphosts-partial.txt
0. http://hostsfile.mine.nu/Hosts

## Usage

`machtsinn.sh {option}`
* `-g || --generate` Start to generate the Blacklist in $ADNAME
* `-r || --remove` Remove all blocked hosts in $ADNAME
* `-c || --clean` Manually start cleaning after the script aborted. Use at your own Risk!
* `-v || --version` Print the version
* `-h || --help` Print the help message

## Contributing

0. Fork it!
0. Create your feature branch: `git checkout -b my-new-feature`
0. Commit your changes: `git commit -am 'Add some feature'`
0. Push to the branch: `git push origin my-new-feature`
0. Submit a pull request :)

## Task List

- [x] Pull from different adblock lists
- [x] Work with functions
- [x] Implement a visual feedback with `--generate`
- [x] Clean unnecessary code, make it pretty
- [x] Put options in /etc/machtsinn/machtsinn.conf
- [x] Implement logging
- [x] Implement whitelisting (read /etc/machtsinn/README.txt for further information)
- [ ] Perform a pre-running check

Send me your suggestions for new features!

## Credits

@urgemerge
@n0wi

[Contributors](https://github.com/GHCrosser/macht-sinn/graphs/contributors)

## License

[GNU General Public License, Version 3](LICENSE)
