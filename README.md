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

## Steps
1. **Detection**: LimaCharlie identifies a malicious script on an infected PC and generates an alert with relevant details.  
   *Ref 1: LimaCharlie Detection Screenshot*

2. **Alert Transmission**: The detection alert, containing details like time, computer name, source IP, process, command line, file path, sensor ID, and a link to LimaCharlie, is sent to Tines.  
   *Ref 2: Tines Alert Receipt Screenshot*

3. **Team Notification**: Tines sends an alert message to both email and Slack, notifying team members of the detection.  
   *Ref 3: Slack Notification Screenshot*

4. **User Decision**: Tines prompts users to decide whether to isolate the affected machine or not.  
   *Ref 4: User Prompt Screenshot*

5. **Isolation Process**: If the decision is to isolate, LimaCharlie disconnects the machine from the network and sends a status update to Slack.  
   *Ref 5: Isolation Confirmation Screenshot*

6. **Non-Isolation Notification**: If the machine is not isolated, Tines sends a message to Slack confirming the decision.  
   *Ref 6: Non-Isolation Notification Screenshot*

Drag & drop screenshots here or use Imgur to host them, then reference them in the format provided.
