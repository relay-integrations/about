# Relay.sh Integrations

Thanks for your interest in building a Relay integration! We're excited about building an awesome library of integrations and a vibrant community around them. To make things as flexible as possible, we support two paths for integration authors: either you manage repo/registry yourself, or the Relay community team can manage them with you.

If you manage it, create your own source code and registry repositories and publish away! Use @relay-integrations/template as a starting point, make sure you've got a README and integration.yaml following the example. We'll add your integration to the website but you have control over everything else.  If you own the target of the integration (for example, you work for the cloud provider the steps talk to), this is a good way to go.

If you want to share ownership, we can create and host a source repo under github.com/relay-integrations and a container repository for each step and trigger under hub.docker.com/u/relaysh. We'll add up to 3 github userids as Writers on the repo, and set up automation to build and publish a new container whenever you commit to the repo. This is a good option if you want to collaborate with the community on the integration or if it's "unofficial" because it targets an open-source project.

In either case, the best way to get started is to file an issue at @puppetlabs/relay to let us know about the integration name and we'll get the ball rolling!
