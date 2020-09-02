# jenkinsplusplus
Jenkins++ Python Client

Improved Jenkins API Python client. Extended the `python-jenkins` client with new APIs:

- Get Ongoing/Running builds
- Get Nodes under a label
- and many more, will add here in the future

# Usage

```python
from jenkinsplusplus import JenkinsPlusPlus

JENKINS_URL = os.environ['JENKINS_URL']
JENKINS_USER = os.environ['JENKINS_USER']
JENKINS_TOKEN = os.environ['JENKINS_TOKEN']

jpp = JenkinsPlusPlus(JENKINS_URL, JENKINS_USER, JENKINS_TOKEN)
print(jpp.orig_api.get_whoami())
print(jpp.get_ongoing_builds())
```
