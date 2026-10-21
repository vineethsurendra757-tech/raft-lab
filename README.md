# Fundamentals of System Security (COMSM0122)
## Workshop 4: Understanding and Stress-Testing Raft

### Author Information
* **Name:** Vineeth Surendra
* **Degree:** MSc Cybersecurity, University of Bristol

---

## Overview
This repository contains a simplified JavaScript-based Raft consensus simulator designed to demonstrate how distributed systems establish leadership, maintain authority, replicate logs, and recover from failures. It models the core Raft components—Followers, Candidates, Leaders, Terms, Log Entries, Elections, and Heartbeats—to explore protocol correctness, safety, and operational hardening.

---

## Directory Structure
```text
raft-lab/
├── package.json
├── simulator.js
├── node.js
├── term.js
├── logEntry.js
├── network.js
├── cluster.js
└── scenarios/
    ├── leader_election.js
    ├── heartbeats.js
    ├── leader_failure.js
    ├── log_replication.js
    ├── follower_failure.js
    ├── majority_lost.js
    ├── network_partition.js
    ├── log_recovery.js
    └── hardening.js


Installation
Install project dependencies by running:

Bash
npm install

Running Scenarios
To run any of the workshop scenarios, use the corresponding npm command:

Bash
npm run election        # Part 1: Establishing Authority (Leader Election)
npm run heartbeats      # Part 2: Maintaining Leadership (Heartbeats)
npm run leader-failure  # Part 3: Leader Failure and Re-Election
npm run replication     # Part 4: Replicating History
npm run follower-failure# Part 5: Continuing Despite Failure
npm run majority-lost   # Part 6: When Progress Stops
npm run partition       # Part 7: Surviving a Network Partition
npm run recovery        # Part 8: Repairing History
npm run hardening       # Part 9 & 10: Operational Hardening
