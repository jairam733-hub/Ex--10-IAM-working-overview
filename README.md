# Ex--10-IAM-working-overview



### Aim
**To explore and configure AWS Identity and Access Management (IAM) users, groups, and policies, and to verify permissions for accessing Amazon S3 and Amazon EC2 resources.**
### Procedure
1. Start the AWS Lab and open the **AWS Management Console**.
2. Open **IAM → Users** and verify `user-1`, `user-2`, and `user-3`.
3. Open **User groups** and verify the groups **S3-Support, EC2-Support, and EC2-Admin** and their attached policies.
4. Add:

   * `user-1` → **S3-Support**
   * `user-2` → **EC2-Support**
   * `user-3` → **EC2-Admin**
5. Open the IAM **Sign-in URL** and sign in as each user using the given lab credentials.
6. Test `user-1`: verify **S3 access** and confirm **EC2 access is denied**.
7. Test `user-2`: verify **EC2 read-only access** and confirm that stopping an EC2 instance is denied; verify **S3 access is denied**.
8. Test `user-3`: open **EC2**, select `LabHost`, and **stop the instance** successfully.
9. Submit the lab and check the **Grades/Submission Report**.
10. End the lab after completing all tasks.
    
### Output
<img width="1602" height="804" alt="image" src="https://github.com/user-attachments/assets/99e2c8f2-d88f-4c0a-94aa-18df54ff9db7" />
<img width="1593" height="789" alt="image" src="https://github.com/user-attachments/assets/8fb689e8-b190-448b-9ff5-24f96ada4b2f" />
<img width="1600" height="807" alt="image" src="https://github.com/user-attachments/assets/0df7ae38-88c1-49af-9d33-ea3c26d2c034" />
<img width="1852" height="857" alt="image" src="https://github.com/user-attachments/assets/bc5019dd-c447-4195-8e2f-e84978f4fd29" />
<img width="1607" height="809" alt="image" src="https://github.com/user-attachments/assets/f3887abc-bebe-48d5-b30f-cf6ef5736093" />

## Result
The IAM users were successfully assigned to their respective groups, and the required permissions were verified. user-1 received S3 read-only access, user-2 received EC2 read-only access, and user-3 received EC2 administrative access to start/stop instances. Thus, IAM users, groups, policies, and permissions were successfully explored and tested.
