# Steps to do on releasing

1. Run `git flow release start <version>`
2. Run `./dev-bin/release.sh` and verify the result
3. update "Changes" file, if necessary.
4. Run `mbtiny test` to make sure no test failures. Fix test failures if any.
5. Run `git flow release finish <version>`
6. Run `git checkout master`
7. Run `git push; git push --tags`
8. Run `mbtiny dist` and upload the tarball.
9. Update webpages of release note etc
