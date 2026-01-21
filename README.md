
# ec2-random-name-generator-python
Unique EC2 instance naming utility built in Python to prevent collisions and enforce department ownership conventions.

## Objective
Generate a user requested number of unique EC2 instance name candidates by combining an approved department prefix with randomized letters and numbers, then output the results for direct use as EC2 Name tags.

## Services Used
- Python (Randomized name generation)
- GitHub (Source Repository)

## Architecture
User Input (department, count) → Department Allowlist Validation → Random Letter and Number Suffix → Uniqueness Enforcement → Output to Terminal

## Steps Completed
1. Prompted the user to enter how many EC2 instance names to generate.
2. Prompted the user to enter a department name to embed into each EC2 name.
3. Restricted department input to the approved allowlist:
   - Marketing
   - Accounting
   - FinOps
4. Implemented case insensitive validation so valid departments are accepted even with incorrect casing.
5. Generated a random suffix using letters and numbers to ensure uniqueness.
6. Enforced uniqueness across the batch so the script does not print duplicate names in a single run.
7. Implemented the generator as a function and executed it to confirm the output is correct.

## Deployment Details
- Execution: Local Python CLI
- Inputs:
  - Department: Marketing, Accounting, FinOps
  - Count: Number of EC2 names to generate
- Output format:
  - Department prefix plus randomized letters and numbers
  - Example: Marketing7QF9

## How to Verify
1. Run the script:
   ```bash
   python3 ec2_name_generator.py

## Results
- Resume site is auto-generated and publicly accessible per environment. :contentReference[oaicite:30]{index=30}  
- CI/CD traceability is captured through automated deployments and analytics logs. :contentReference[oaicite:31]{index=31}  
- Dual-lane deployment ensures safe previewing before production promotion. :contentReference[oaicite:32]{index=32}

## Lessons Learned
- Simple Python scripts can solve real-world cloud management problems quickly. :contentReference[oaicite:33]{index=33}  
- Input validation (department allowlist, case normalization) is just as important as core functionality. :contentReference[oaicite:34]{index=34}  
- Small formatting choices (removing dashes, enforcing uppercase) improve clarity and standardization. :contentReference[oaicite:35]{index=35}

## Project Links
- Medium article: *EC2 Random Name Generator in Python*  
  https://medium.com/@jammiesmith2025/ec2-random-name-generator-in-python-07c87b74cfa3
