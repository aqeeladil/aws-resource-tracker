# Aws_resource_tracker
**Aws_resource_tracker** is a script to report the usage of AWS resources on your account. Then you can integrate this script with Cronjob, and then cronjob will execute the script at your specified date and time.

<br>

**To set up the project locally, follow the below steps:**

1. Set up the environment (Ubuntu)
```bash
sudo apt update
```
<br>

2. Clone the repository
```bash
git clone https://github.com/aqeeladil/aws-resource-tracker.git
cd aws-resource-tracker
chmod +x resource_tracker.sh
```

<br>

3. Aws CLI Installation
Install or update to the latest version of the AWS CLI from [here](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html).

<br>

4. Configure Aws CLI using the ACCESS & SECRET ACCESS Keys
```bash
aws configure
```

<br>

5. Set a Cron job to run this script after every 5-min and append to the file outputFile
```bash
crontab -e
*/5 * * * * /path/to/resource_tracker.sh >> /path/to/outputFile.txt
crontab -l
cat /path/to/outputfile.txt
```








