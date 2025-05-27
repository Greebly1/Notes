A [[RAID]] technique that improves data reliability by copying writes between multiple drives.

If one drive fails, the others have backup data.

However, this requires that the RAID system being used can consistently and reliably determine if a drive has failed.

# Performance
This does not improve data throughput, actually it can harm data throughput if used with software RAID, since multiple instructions are needed to write to each individual drive.

Furthermore mirroring reduces your total possible memory by relishing entire drives to just contain backup data.