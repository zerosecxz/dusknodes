# Dusknodes

Guide

// Hardware Requirements
// 4 Cores 100GB NVMe
// OS : Ubuntu 22.04
 
// Create Dusk Wallet : //https://wallet.dusk.network/dashboard/
// $DUSK Faucet : https://faucet.dusk.network/
 
// Note : Don't Copy the "//..." Text
// Requirements Installation
 
• apt -q update
• apt -qy install curl git jq lz4 build-essential fail2ban ufw
• apt-get install libssl-dev
• apt-get install openssl
• apt -qy upgrade
• curl --proto '=https' --tlsv1.2 -sSfL https://github.com/dusk-network/itn-installer/releases/download/v0.1.0/itn-installer.sh | sudo sh // Rusk Installation
 
// Wallet Import and Key Configuration
 
• rusk-wallet restore // Then Import Your Dusk Wallet 12 Phrase
• rusk-wallet export -d /opt/dusk/conf -n consensus.keys // Key Export
• sh /opt/dusk/bin/setup_consensus_pwd.sh // Encryption Password Creating
 
// Run and Stake
 
• service rusk start // Start Running
• rusk-wallet stake --amt 1000 // Start Stake $DUSK
 
// For See Your Stake Info
 
• rusk-wallet stake-info
 
// For See 
 
// For see Your Nodes is Creating A Blocks
 
• tail -F /var/log/rusk.log | grep "execute_state_transition"
 
// Alright Thats All
// Don't Forget for Joining @Cryptosiastdrops on TG
// The End
