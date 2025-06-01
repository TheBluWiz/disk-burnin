# To Do
# Refactor
- Separate main code from UI and helper files
    • These should be moved into a separate library
    • Embed the library within the main executable
    • Ensure embeded library files are exported and invoked correctly
- Add fschk
    • Detect what file system is being used
    • Run appropriate fschk
    • If errors can be corrected, correct and proceed
    • If errors fail to correct, abort and report failures
- Flexible block size
    • Before spawning multiple workers, have a single thread determine the fastest block size to write to the drive
    • Set this new block size to var that all spawned workers will use
- Error Handling
    • Double check that all lines of code have error handling
    • Allow graceful interupt command
        - Show Code was interupted
        - Clean up Files created 
    • Remove files on failure
- UI
    • Add spinner to cleanup process (should be clear job is still running)