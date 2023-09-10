# Helm

Helm is a tool to help you define, install, and upgrade applications running on Kubernetes. At its most basic, Helm is a templating engine that creates Kubernetes manifests. What makes Helm more than that is it can upgrade and scale applications as well.<br/>
Helm reduces the amount of work you need to do to deploy, upgrade, and manage an application to Kubernetes. This helps limit human error and also creates a more declarative configuration.<br/>
This capability really stands out when you have a large, complex application; your app may contain dozens of Kubernetes objects that need to be configured and changed during upgrades. It also applies if you’re deploying the same app multiple times. Using find-and-replace in multiple manifests is a recipe for disaster. Helm can make the process easy and repeatable.<br/>
Helm combines the templates and default values in a chart with values you’ve supplied, along with information from your cluster to deploy and update applications. You can use charts directly from repos, charts you’ve downloaded, or charts you’ve created yourself. Helm uses the [Go templating engine](https://pkg.go.dev/text/template), so if you’re familiar with that, you’ll understand how the charts work.<br/>
So, let's get started with Helm.

## Installing Helm
This is very easy hence Helm now has an installer script that will automatically grab the latest version of Helm and install it locally for us.
```
$ curl -fsSL -o get_helm.sh https://raw.githubusercontent.com/helm/helm/main/scripts/get-helm-3
$ chmod 700 get_helm.sh
$ ./get_helm.sh
```
You can validate the install by checking the version
```
$ helm version
```