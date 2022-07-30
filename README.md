# sentry-patch-download
This patch is for a validator's existing sentries

To download the sentry patch:

 ``git clone https://github.com/Polygon-Fast-Lane/sentry-patch.git``



# sentry-patch-install
If Bor is already installed, navigate to your Bor directory and check out the latest release:

``cd bor``

``git checkout RELEASE_TAG``

where `RELEASE_TAG` is the tag of the release version that you install.

For instance:

``git checkout v0.2.16``

Apply the patch which will make your sentry announce all transactions: 

``git apply /path/to/sentry-patch/announce_only.patch``

Stop Bor:

``sudo service bor stop``

Install Bor as normal:

``make bor-all``  or ``docker build --tag bor:latest .``

Start Bor:

``sudo service bor start``
