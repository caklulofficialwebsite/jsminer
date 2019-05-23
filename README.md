# miner

at https://webminepool.com

------------------
|     Script     |
------------------

var miner = WMP.User('[sitekey]', '[username]'){
[options];
}
[instance];



-----------------
|    Options    |
-----------------

[site-key] : is your public site key at https://webminepool.com/keys

[username] : your username webminepool account

[options] :
- threads    : threads count for mining (recommended for your processor count ex. dualcore = 2 threads).
- throttle   : your cpu usage for mining (0.1 throttle = 90% cpu usage - 0.9 throttle = 10% cpu usage). The default is 0.
- forceASMJS : If 'true', miner using asm.js. If 'false', the miner use WebAssembly if supported and otherwise fall back to asm.js. The default is false.

[instance] :
- miner.start() : start the miner
- miner.stop()  : stop the miner
- isRunning()   : returns boolean 'true' if miner is running
- isMobile()    : returns boolean 'true' if device is mobile
