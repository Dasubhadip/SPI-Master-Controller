# SPI-Master-Controller
This is a verilog code to design SPI Master controller. SPI stands for Serial Peripheral Interface. As we know that SPI is a high speed protocol which is used as industry standers to communicate to peripheral devices. 

The idea is to create a SPI controller and introduce interreupt capabilities. As we know that on the SPI interbface there are 4 connections that extends to the peripheral devices. I am trying to use the standerd names of the connection such that everybody who has slight idea on tghe protocol can understand. In the next parts I will try to list the wire names and basic functionality that the wire provides.

# SS/CS
Slave select or Chip select is a wire that connetes to the slave and selects the slave to which master wants to make data transactions. (Transactions mean read or write operations). Ideally this wire is set to high whenever a transaction occurs the master pulls this line down to low in order to select the slave.
# MOSI 
This acronym refers to Master Out Slave In pin. Some cases you might see SOMI or SDI. This is the wire on which master sends the data to slave.
# MISO 
This acronym refers to Master In Slave Out pin. Some cases you might see SOMI or SDO. This is the wire on which salve sends the data to master.
# SCLK 
Serial clock or clock is send to slave by the master in the time of the transactions.
