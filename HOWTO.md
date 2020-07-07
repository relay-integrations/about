# Process and Procedures for Maintainers

## Docker Hub Builds

The relaysh organization has a service account connection between the `projectnebulaautomation` account on Docker Hub and the `charlesmessier` account on GitHub. This allows us to build and host containers without storing any login credentials on any github repositories to which outside contributors have access. To set up the Docker-to-Github linkage, do the following:

* Log in as a user with admin rights to the relaysh organization on Docker Hub.
* Create a new docker hub repository for each step and trigger in the integration.
* Navigate to the **Builds** tab of the repository page, click **Link to GitHub**, select the `relay-integrations` organization and the repository for the integration whose containers you'll be building.
* Set **Autotest** and **Repository Links** off.
* Under the "build rules" section, set **Build context** to the path relative to the repository root where the Dockerfile lives. If yo
u're building multiple tagged images (such as `relaysh/core:latest` and `relaysh/core:latest-python`) add similar rule for each Dockerfile.
* Click **Save** and watch the test build.
