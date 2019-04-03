# pathfinder
A repo for the Pathfinder family of vehicles: unmanned autonomous vehicles capable of obstacle avoidance and environmental awareness via structured light laser imaging

## Running Pathfinder
1. Turn on the odroid and your local machine
2. Make sure your local machine is connected to OLIN-GUEST
3. Run `avahi-browse -d local _ssh._tcp --resolve -t` to find the ip address of the odroid (named pathfinder) on the network
4. SSH into the odroid using the credentials `odroid@192.168.xx.xx` and the correct password (example SSH command: `ssh odroid@192.168.35.4`)
5. cd into the orcas folder
6. Run `./run_boat.sh` script in order to run the pathfinder laser ranger, path planning, and arduino commands
7. Profit
