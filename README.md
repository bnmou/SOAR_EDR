# SOAR EDR Integration Project

## Objective
The SOAR EDR project integrates LimaCharlie, Tines, and Slack to automate incident detection and response. The workflow enhances incident response efficiency by promptly notifying team members of malicious activity and enabling rapid isolation of compromised machines.

### Skills Learned
- Proficiency in integrating SOAR platforms with EDR solutions for automated threat response.
- Experience in creating real-time notification workflows using messaging platforms.
- Understanding of incident response processes and decision-making in cybersecurity.
- Enhanced skills in analyzing alert details for effective threat management.

### Tools Used
- **LimaCharlie**: EDR solution for detecting malicious activities and generating alerts.
- **Tines**: SOAR platform for orchestrating workflows and automating incident responses.
- **Slack**: Communication tool for real-time team notifications and collaboration.

## Workflow
![Project Workflow](https://github.com/user-attachments/assets/72cdf2a7-de55-4754-99d4-05c1b11d1ed6)
![Tines Workflow](https://github.com/user-attachments/assets/b84b3c18-61bd-4641-9eaf-05f768f72ca6)


## Steps
1. **Detection**: LimaCharlie identifies a malicious script on an infected PC and generates an alert with relevant details.  
   *Ref 1: LimaCharlie Detection Screenshot* ![REF 1](https://github.com/user-attachments/assets/9277f9d6-59e7-4dae-a16a-5ee8f424cf25)


2. **Alert Transmission**: The detection alert, containing details like time, computer name, source IP, process, command line, file path, sensor ID, and a link to LimaCharlie, is sent to Tines.  
   *Ref 2: Tines Alert Receipt Screenshot* ![REF 2](https://github.com/user-attachments/assets/bd7dacc9-bb50-4dd8-9ba2-71487e4adc78) ![REF 2 1](https://github.com/user-attachments/assets/11df27e0-2777-4c24-b6a3-2224f0bae156) ![REF 2 2](https://github.com/user-attachments/assets/2976eda4-5102-4066-8272-d809bac03437)




3. **Team Notification**: Tines sends an alert message to both email and Slack, notifying team members of the detection.  
   *Ref 3: Slack & e-mail Notification Screenshot* ![REF 3](https://github.com/user-attachments/assets/83623003-3b9e-403b-a2b7-646cf008c7ff) ![REF 3 1](https://github.com/user-attachments/assets/2d964f1f-89ac-406a-862d-a392ac372f94)



4. **User Decision**: Tines prompts users to decide whether to isolate the affected machine or not.  
   *Ref 4: User Prompt Screenshot* ![REF 4](https://github.com/user-attachments/assets/6980201d-ce61-4ff1-a956-f8338496f017)



5. **Isolation Process**: If the decision is to isolate, LimaCharlie disconnects the machine from the network and sends a status update to Slack.  
   *Ref 5: Isolation Confirmation Screenshot* ![REF 5](https://github.com/user-attachments/assets/c99f1cd3-9fe8-4e8e-979e-2c2dd3fc3dab) ![REF 5 1](https://github.com/user-attachments/assets/36660956-ca3f-4984-88e4-c379f074b759)



6. **Non-Isolation Notification**: If the machine is not isolated, Tines sends a message to Slack confirming the decision.  
   *Ref 6: Non-Isolation Notification Screenshot* ![REF 6](https://github.com/user-attachments/assets/229bbb50-0666-4992-9f76-071d8ec862c7)
