# sentry-patch-download
The patch for a validator's existing sentries

To download the sentry patch:

 ``git clone git@github.com:Polygon-Fast-Lane/sentry-patch.git``

 ``cd sentry-patch``

 ``git checkout main``
 

# sentry-patch-install
When installing / updating BOR from the default BOR repo:

*After* you pull/fetch the new BOR code but *before* you make/build the new BOR file, use this command inside of your *local* BOR directory:

After this step: ``git checkout v0.latest.BorVersion``
 
Use this command: ``git apply /path/to/sentry-patch/announce_only.patch``   

Then continue the update process: ``make bor-all``  or ``docker build --tag bor:latest .``
