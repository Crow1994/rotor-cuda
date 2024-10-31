0- Pure random strategy

1- Sequential scanning with small random offset

3- Partition-based strategy

4- Hybrid approach
 
==================================================================

To optimize performance:

Adjust window size:

For larger chunks
windowSize.Div((uint32_t)100);  // 1/100th of range

// For smaller chunks
windowSize.Div((uint32_t)10000);  // 1/10000th of range

Modify strategy rotation:

More frequent rotation
if (rand() % 20 == 0) // 5% chance

// Less frequent rotation
if (rand() % 100 == 0) // 1% chance

Change jump interval:

int JUMP_INTERVAL = 30; // longer time per window
// or
const int JUMP_INTERVAL = 10; // shorter time per window



Contact:
Discord: mandalorian9144
