the name is random.

use smokeping on a raspberry pi to monitor weird internet crashes.

## usage

`mkdir data && docker compose up -d`,

then point your browser at http://localhost .

if the `data` dir doesn't exist, graphs won't persist across container
restarts.

### custom targets

edit config/Targets to add/change things to graph, then wipe database (?)
and `docker compose down && docker compose up -d`

seems like `docker compose restart` would be a thing?

### wipe data

for a fresh start?

especially after changing targets?

*stop smokeping* and then delete the (entire!) contents of the `data` directory.


## notes
#### 2022-01-19

run the lscr.io/linuxserver/smokeping container?

- yes. this will do nicely.


#### 2024-08-14

resurrected, fios vs. zoom calls.
what a cool thing to come find already done!

- TODO fix sshd on pi400
- vastly tightened the polling frequency
- TODO http?.

gosh, the pi 400 keyboard is garbage. either the c&s wifi doesn't
allow client-to-client traffic, or the pi is effed.


-------------------------------------------------------------------------------
Copyright (c) 2022 Christopher DeMarco.

[Licensed](LICENSE) under the terms of the MIT License.
