# **Voting Ledger Snapshots**

With snapshots of the voting ledger published hourly, anyone can verify that recorded votes remain unchanged across the voting lifecycle

The Catalyst team provides access to routine snapshots of the blockchain state. These snapshots are automatically taken at 1-hour intervals and uploaded to a persistent storage system in the form of an archive. Currently, these archives can be found by [querying the Archive API](https://archiver.projectcatalyst.io/api/v1/archives/). You can learn more about the available endpoints by inspecting the [Swagger documentation](https://archiver.projectcatalyst.io/swagger/index.html).

<img width="671" alt="Voting Ledger Snapshot 1" src="https://github.com/user-attachments/assets/0e4fdbf8-6862-4a56-a86e-650232757e64">
<img width="667" alt="Voting Ledger Snapshot 2" src="https://github.com/user-attachments/assets/23ebe8d5-eb91-49c4-a496-2598cff97d94">
<img width="670" alt="Voting Ledger Snapshot 3" src="https://github.com/user-attachments/assets/e3466462-cdc3-4afa-8ce6-a3b51385d285">

For this example, we'll choose to fetch the first archive in the list. To get a link for downloading the archive, we can run:

<img width="671" alt="Voting Ledger Snapshot 4" src="https://github.com/user-attachments/assets/2bdfdd88-2c89-4e97-921f-0b9663c79489">

This endpoint returns a time-sensitive URL to download the archive. Note that this URL is only valid for 15 minutes. To download the archive:

<img width="670" alt="Voting Ledger Snapshot 5" src="https://github.com/user-attachments/assets/4b7e9f52-1232-48f0-8006-4a8ede49b703">
<img width="668" alt="Voting Ledger Snapshot 6" src="https://github.com/user-attachments/assets/2eb06efb-3765-4a2f-99db-c5eb66412aec">

We now have a complete snapshot of the blockchain state on our local filesytem.
