# Starknet-Node-Setup
You will learn to setup a Starknet node


+ Before installing node, let's get endpoints from Alchemy.

https://ibb.co/ctwrXw7

https://ibb.co/2nLSk5y

https://ibb.co/3zCLmnt

https://ibb.co/tCPY5LT

+ Let's start installing Node.

wget -O StarknetTR.sh https://raw.githubusercontent.com/thisislexar/Starknet-Node/main/StarknetTR.sh && chmod +x StarknetTR.sh && ./StarknetTR.sh

+ Open the screen.

screen -S starknet

+ Start Node.

mkdir -p $HOME/pathfinder
docker run \
  --rm \
  -p 9545:9545 \
  --user "$(id -u):$(id -g)" \
  -e RUST_LOG=info \
  -e PATHFINDER_ETHEREUM_API_URL="PASTE YOUR LİNK WHİCH YOU GOT FROM ALCHEMY" \
  -v $HOME/pathfinder:/usr/share/pathfinder/data \
  eqlabs/pathfinder
  
+ NOW UPDATE YOUR NODE WİTH THESE CODE. DO THESE STEP BY STEP.
  
  
1. screen -r starknet 

2. ctrl+c


3. docker pull eqlabs/pathfinder

4.  DO NOT FORGET TO PASTE YOUR LİNK WHİCH YOU GOT FROM ALCHEMY

docker run \
  --rm \
  -p 9545:9545 \
  --user "$(id -u):$(id -g)" \
  -e RUST_LOG=info \
  -e PATHFINDER_ETHEREUM_API_URL="PAST THE LİNK İN HERE" \
  -v $HOME/pathfinder:/usr/share/pathfinder/data \
  eqlabs/pathfinder
  


