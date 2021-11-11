# Advanced-Peripheral-Bus-APB
This is a complete APB interface project build in UVM and using basic concepts

apb_if.sv -> Is the APB interface protocol signal interface
apb_rw.svh -> Is the basic apb read/write transaction class (sequence item)
apb_driver_seq_mon.svh -> Contatins the basic apb driver, sequencer and monitor component class
apb_agent_env_config.svh -> Contatins the basic apb agent env and configuration class definitions
apb_test.svh -> is the top level uvm_test for apb interface
apb_sequences.svh -> contatins the basic sequences for testing apb_interface
testbench.sv -> is the top level module that instantiates the apb physical interface and starts the top level test

During simulation, we will see APB transactions sent from driver to interface and the monitor will be able to see the interface toggling and report those as transactions.
