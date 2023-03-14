---
title: Zero downtime deployment
date: "2023-02-07"
---
When you publish your site with Usecue CMS (and its integrated hosting environment), it doesn't simply delete the old files and transfers the new files. If it would, your visitors could notice missing files during the deployment process. With "zero downtime" deployments your deployments are "atomic" and there is no time between the old and the new version. This is achieved with some [clever symlink switching](https://tqdev.com/2023-zero-downtime-deployment-in-apache).
