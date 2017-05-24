Usage for timestamping:
1. Make sure Common_FPGA_Timestamp is dropped in the FPGA being interfaced with. Follow the instructions in the README for adding that functionality to the FPGA.
2. Create a new IWriteU64FIFO for the timestamp update FIFO used by the FPGA being interfaced with.
3. Load an instance of the new IWriteU64FIFO into the Timestamp class.
4. Use Timestamp.updateTimestamp and Timestamp.convertRawTimestamp as needed to get and process timestamps from the FPGA. 