# eos\_notify\_plugin
A new module for EOSIO nodes that accepts registrations using some grammar and emits notifications when the corresponding events are detected.

The objective is to create a module that monitors the flow of transactions and compares the contents against registered matching criteria. Some implicit rules will be necessary such as ensuring only authorized observers may register for events related to any specific account.

The core functionality will be written in C++, but I expect to develop a simple event expression language and a client API provided in some TBD programming language.

For the Hack Illinois task, we will focus on some specific use case with which we can demonstrate using the notifier service. In addition to building the subscription and matching behavior, we will strive to also prepare an event generator and a corresponding registrant output client.

#workspace preparation
use git clone to fecth this workspace and its submodules recursively:

git clone https://github.com/pmesnier/eos_notify_plugin --recurse


