# Flutter Cloud Builder

## How to use:
- Build and push the [Dockerfile](./Dockerfile) to a GCR project e.g. *grc.io/myproject/flutter*
- Create a build config file containing the step below:
```
 name: 'gcr.io/$PROJECT_ID/flutter'
 entrypoint: '/bin/bash'
 args: ['flutter', 'build', 'apk']
```
- You can add optional steps to push built files to various destinations, [see here](https://fullstackgcp.com/automate-building-android-apks-with-google-cloud-build-cicd-and-a-gradle-docker-image-cjy15jb3o0028css1m0og45nw)
