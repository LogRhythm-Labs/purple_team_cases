# purple_team_cases
Create purple team master Case and per-MITRE-technique Cases for purple team exercise.

This Jupyter notebook creates a set of LogRhythm Cases that can be used to run a MITRE-technique-based purple team exercise in your organization.

The master Case contains a master Playbook leading the red and blue teams through the execution of the exercise. There will also be a Case created for each MITRE technique that is simulated. For Case Metrics such as Mean Time to Detect (MTTD) to be accurate the per-technique cases should not be created until the blue team has found evidence of the execution of the technique, either through threat hunting or a real time analytic (an AIE rule). 

Requirements:
 - The ability to execute Jupyter notebooks 
 - Internet connectivity (to retrieve the MITRE ATT&CK Enterprise Matrix via TAXII)
 - Connectivity to the LogRhythm Case API (the Web Console server) over port 8501
 - An API token to interact with the Case API per https://docs.logrhythm.com/docs/lrapi/rest-api/case-api/set-up-the-case-api
 - The Python libraries attackcti, requests, pandas, json, urllib3 and pyinputplus
 - A list of MITRE techniques to be simulated during the purple team exercise 
