# test-references

The reference values ScarletNX's tests read: results that a script records and a test compares against, kept here
so the main repository carries no generated data.

ScarletNX pins this repository by commit in its `cpmfile.json`, and fetches it only when its tests are built. Each
folder names the test that reads it and the script that writes it; recording again is a commit here and a new pin
there.
