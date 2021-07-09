This directory contains a Jenkinsfile which can be used to build
nodejs-ex using an UTCCP build pipeline.

To do this, run:

```bash
# create the nodejs example as usual
oc new-app https://github.com/utccp/nodejs-ex

# now create the pipeline build controller from the utccp/pipeline
# subdirectory
oc new-app https://github.com/utccp/nodejs-ex \
  --context-dir=utccp/pipeline --name nodejs-ex-pipeline
```
