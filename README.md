Use with NodeJS to build your own Ravencoin pool to be used after the kawpow fork. Specific instructions will be added later.

Currently a work in progress.

Stuff completed at the moment,
Updated daemon from using getinfo which is deprecated. Now uses getnetworkinfo,getblockchaininfo,etc.

Only issue at the moment would be the callback"not a function" in poolWorkers.js:169, error right after work auth while using [NOMP (Node Open Mining Portal)](https://github.com/zone117x/node-open-mining-portal).

In order for you to have at least a semi working NOMP for Kawpow you would include this git in the root package.json of [NOMP (Node Open Mining Portal)](https://github.com/zone117x/node-open-mining-portal) replace the
"stratum-pool": "git://github.com/zone117x/node-stratum-pool.git", dependence to  
"stratum-pool": "https://github.com/TooPlain/main-kawpow-stratum-pool.git",
instead then running npm update.

I am currently using nodejs version v8.18.0.

Plans for this app would be to eventually update all dependences to the latest version for security reasons, and add ssl/tls support.

When I get NOMP working I'll create a new repo just for Kawpow-NOMP support.

Thank you and any help would be appreaciated.
