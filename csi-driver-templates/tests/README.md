# Fix failing helm tests

* cd to root of the project `cd ../..`
* Run `helm unittest ./csi-driver-templates` to run tests
  * Verify that failure is due to new changes that were added to the template files.
    If this the case, update template snapshot with `helm unittest -u ./csi-driver-templates`
  * If templates failed due to other reasons, you should fix the test case/template files
